# Jogos Bem Feitos: Visão Geral do Produto

> Última atualização: 2026-09-29

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

## 4. Funcionalidades da plataforma (descrição oficial, 2026-09)

O Jogos Bem Feitos reúne ferramentas para consultar resultados, gerar e organizar
jogos, cadastrar apostas e gerenciar participantes e créditos. A plataforma facilita
o acompanhamento das apostas e o compartilhamento das informações com os jogadores.

> Parte do que aparece no roadmap abaixo (apostas, jogadores e saldos, grupos de
> jogos, resultados, extensão) já está descrito aqui como funcionalidade disponível.
> Em caso de conflito, vale esta seção.

### Resultados de todas as modalidades

Consulte os resultados dos concursos das modalidades disponíveis na plataforma em um
único lugar. Visualize os números sorteados e as informações do sorteio para
acompanhar os concursos e conferir seus jogos.

### Extensão para o Chrome

Acesse recursos do Jogos Bem Feitos diretamente pelo navegador, por meio de uma
extensão com painel lateral e acesso mediante login. A extensão auxilia na inserção
dos jogos no ambiente de apostas, com controle dos jogos já inseridos e dos que ainda
estão pendentes.

### Cadastro e gerenciamento de apostas

Cadastre e organize suas apostas, reunindo os jogos, os participantes, as cotas e as
informações do concurso. Acompanhe os dados de cada aposta desde sua preparação até a
conferência do resultado.

#### Link público da aposta

Compartilhe uma página de consulta com todas as informações da aposta. Quem receber o
link poderá visualizar os jogos, os participantes, as quantidades, os dados do sorteio
e a aba de resultado.

A página apresenta as informações em modo de visualização, sem opções de edição,
facilitando o acompanhamento pelos participantes.

#### Textos para compartilhar no WhatsApp

Gere textos prontos para copiar e enviar pelo WhatsApp, facilitando a comunicação com
os jogadores:

- **Resumo completo da aposta:** apresenta os detalhes para acompanhamento do grupo.
- **Resumo resumido:** reúne as principais informações em uma mensagem mais curta.
- **Lista de jogadores e saldos:** informa os participantes e seus créditos atuais.
- **Resultado da aposta:** apresenta a quantidade de jogos premiados, o valor recebido
  e o valor por cota.

#### Cálculo automático do resultado

Confira os jogos cadastrados a partir do resultado do concurso. A plataforma calcula
os acertos e consolida as informações de premiação da aposta, permitindo acompanhar os
jogos premiados, o total recebido e a distribuição por cota.

### Cadastro de jogadores

Cadastre os jogadores para organizar os participantes das apostas e acompanhar suas
participações. Mantenha os registros centralizados, facilitando a identificação de
quem participa de cada aposta.

#### Gerenciamento de créditos

Controle os créditos de cada jogador, acompanhe os saldos disponíveis e registre as
movimentações. Esse recurso facilita a organização dos valores utilizados nas
participações e a consulta do saldo individual.

### Cadastro de jogos

Cadastre e mantenha seus jogos organizados na plataforma. Consulte as combinações
registradas e vincule os jogos às apostas, facilitando a preparação e a conferência
dos concursos.

### Grupos de jogos

Organize conjuntos de jogos em grupos para facilitar sua identificação e utilização.
Separe as combinações conforme seus próprios critérios, como estratégia ou finalidade,
mantendo uma estrutura mais prática para consultar e selecionar os jogos.

### Gerador de jogos com IA

Gere combinações com o auxílio de inteligência artificial e das estratégias
disponíveis na plataforma, como geração aleatória, repetição equilibrada,
probabilidade, tendência histórica e perfis de combinações.

O recurso facilita a criação e a organização dos jogos conforme a estratégia
escolhida. As análises e os padrões históricos não garantem premiação nem permitem
prever os números dos próximos sorteios.

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
