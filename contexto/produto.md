# Jogos Bem Feitos: Visão Geral do Produto

> Última atualização: 2026-08-20

## O que é

Jogos Bem Feitos é uma plataforma de apoio ao jogador de loterias que usa Inteligência
Artificial para gerar jogos com base em estratégias estatísticas configuráveis,
analisando histórico de concursos, frequência de dezenas, atrasos e tendências para
sugerir combinações mais alinhadas ao perfil que o usuário escolher.

A plataforma nasce em três frentes de acesso (**Web**, **Extensão de navegador** e
**Aplicativo mobile**), além de uma **área administrativa** para gestão interna.

## 1. Gerador de Jogos por IA (funcionalidade central, já implementada)

O coração do produto: o usuário escolhe a modalidade, a estratégia e a quantidade de
jogos desejada, e a IA gera as combinações, avaliando e pontuando cada jogo antes de
entregá-lo.

### Como funciona, na prática

- **Escolha a modalidade** entre as 9 loterias suportadas: Mega-Sena, Quina, Lotofácil,
  Lotomania, Dupla Sena, Timemania, Dia de Sorte, Super Sete e +Milionária, cada uma
  com suas regras próprias de universo numérico e quantidade de números por jogo.
- **Escolha a estratégia**: cada estratégia tem um card com resumo e um "Saiba mais"
  com a explicação completa:
  - **Aleatório equilibrado**: jogos livres, sem se basear em concursos passados,
    buscando apenas equilíbrio básico (pares/ímpares, faixas, soma) e diversidade
    entre os jogos gerados.
  - **Repetição Equilibrada**: reproduz uma técnica real de fechamento, repetindo de
    7 a 11 números do último concurso, com cobertura de dezenas e soma dentro de
    faixas estatisticamente testadas.
  - **Equilíbrio Estatístico**: perfil configurável de pares/ímpares, primos, números
    consecutivos, soma e média.
  - **Tendência Histórica**: classifica as dezenas em "quentes", "neutras",
    "atrasadas" e "frias" com base na frequência recente e monta os jogos numa
    proporção balanceada entre elas.
  - **Similaridade Histórica**: analisa os últimos 100 concursos, identifica os
    padrões estruturais mais recorrentes e distribui os jogos com base neles.
- **Escolha a quantidade**: de 1 a 50 jogos por geração, com seletor de quantos
  números por jogo quando a modalidade permite variar.
- **Geração em tempo real**: a tela mostra o progresso ao vivo ("Buscando os melhores
  jogos: X de Y bons encontrados até agora…") enquanto a IA processa em segundo
  plano.
- **Score de aderência**: cada jogo entregue recebe uma pontuação de 0 a 100%
  mostrando o quanto ele se encaixa nos critérios da estratégia escolhida, com um selo
  colorido (verde/amarelo/vermelho) e detalhamento dos critérios avaliados. O score
  nunca é usado para bloquear um jogo, é só uma referência de qualidade para o
  usuário decidir.
- **Adição rápida**: cada jogo pode ser adicionado individualmente ou tudo de uma vez
  ("Adicionar todos"), com proteção contra duplicidade.

## 2. Planos de Assinatura

Três planos com cota diária de gerações por IA, quantidade de jogos salvos, jogadores
vinculados e recursos adicionais (agrupamento de jogos, análise de apostas, chat
inteligente):

| Plano   | Preço          | Gerações IA/dia | Jogos salvos | Jogadores | Recursos extras   |
|---------|----------------|------------------|--------------|-----------|--------------------|
| Free    | Gratuito       | 10/dia           | até 50       | N/A       | N/A                |
| Basic   | R$ 29,90/mês   | 50/dia           | até 1.000    | até 5     | Agrupamento + Chat |
| Premium | R$ 69,90/mês   | 1.000/dia        | até 50.000   | ilimitado | Tudo liberado      |

(preços também disponíveis em planos semestral e anual com desconto)

## 3. Autenticação e segurança

Login seguro via JWT, com controle de acesso por plano contratado.

## Roadmap em desenvolvimento

A plataforma está em construção ativa. Abaixo, as próximas entregas organizadas por
área, ótimo material para comunicar "o produto está vivo e crescendo":

### 🌐 Web

- **Assinatura**: exibir plano atual e upgrade direto no header; bloqueio de
  funcionalidades sem plano ativo; regra de downgrade automático em caso de pagamento
  em atraso; cancelamento pelo próprio usuário.
- **Apostas**: fluxo completo de cadastro de aposta (jogadores, jogos e geração por IA
  integrados); análise de cada aposta criada; agendamento automático de inserção de
  jogos com geração de PIX.
- **Sorteios**: carga histórica de todos os concursos já realizados.
- **Chat Inteligente ("Trevin")**: testes de fluxo de tool-calling com confirmação de
  ações; fallback entre provedores de IA; respostas via streaming (SSE).
- **Jogadores**: confirmação de e-mail no convite; gestão de jogadores e saldos.
- **Jogos**: CRUD completo de jogos; agrupamento de jogos em grupos personalizados;
  análise individual de cada jogo; página dedicada ao Gerador por IA.
- **Loterias**: página com visão completa de cada loteria e seus resultados.
- **Minha Conta**: troca segura de e-mail e senha; troca de foto de perfil;
  configuração de planos/preços por modalidade.
- **Cadastro**: indicador de força de senha.
- **Auditoria**: registro de ações em log de auditoria.
- **Site**: ajustes finos de contraste em textos e ícones de badges.

### 🧩 Extensão de navegador

Bloqueio de funcionalidades sem login na Caixa; página de instruções de instalação;
abas de navegação (Apostas, Jogos, Jogadores, Chat); e réplica das principais telas do
Web (apostas, jogadores, jogos, gerador de IA, análise, agrupamento, assinatura,
chat).

### 📱 Aplicativo mobile

Storybook de componentes para React Native; telas de cadastro, login e home; réplica
completa das áreas de assinatura, chat inteligente, apostas (incluindo inserção
automática de jogos), jogadores, jogos, loterias, minha conta e extensão.

### 🛠️ Administrativo

Tela de gestão de usuários e assinaturas; configuração de preços por modalidade
(valor base e incremento por dezena); gestão manual de concursos, com opção de marcar
como apurado.
