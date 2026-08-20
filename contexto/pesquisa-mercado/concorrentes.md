# Mapeamento de Concorrentes — Mercado Brasileiro de Ferramentas para Apostadores de Loterias da Caixa

Pesquisa realizada via WebSearch e WebFetch em agosto/2026. Todas as informações são baseadas em fontes reais citadas; quando não foi possível confirmar um dado, isso está marcado explicitamente como "não confirmado".

---

## PARTE 1 — CONCORRENTES DIRETOS (geradores de jogos, estatística, fechamento/desdobramento)

### 1. LotoAI

| Campo | Detalhe |
|---|---|
| Produto | LotoAI |
| URL | https://www.lotoai.com.br/ (produto: /produto, planos: /planos, API: /api-publica) |
| Plataforma | Web |
| Modalidades | Mega-Sena, Lotofácil, Quina e "todas as loterias" da Caixa |
| Público-alvo | Apostadores que buscam ferramenta analítica/geradora com apelo tecnológico |
| Proposta principal | "Gerador de Jogos com IA para Loterias — Simulador e Análise"; posiciona-se explicitamente como ferramenta de análise/entretenimento, não site de apostas |
| Geração de jogos | Sim |
| IA | Comunicação forte de IA: nomeia "modelos" próprios (ex. "LOT-1-Mini"), fala em processar "milhares de concursos históricos" com "machine learning" — terminologia de produto de IA, mas sem detalhamento técnico verificável publicamente |
| Estatísticas | Sim (dashboard analítico no plano Ultimate) |
| Fechamentos | Não confirmado explicitamente na varredura, mas há "pacotes de jogos" com planilhas |
| Gestão de jogos | Parcial (pacotes/planilhas) |
| Conferência | Não confirmado |
| Automação com Caixa | Não encontrada evidência |
| Diferenciais | API pública REST para desenvolvedores (resultados, estatísticas, sugestões via IA); modelo de preço vitalício (não recorrente) é incomum no setor |
| Preço | Normal R$ 12,90 / Plus R$ 21,90 / Ultimate R$ 99,90 — **pagamento único, acesso vitalício**; pacotes avulsos a partir de R$ 29,90 |
| Modelo de monetização | Compra única (freemium com upsell de planos vitalícios) |
| Pontos fortes | Diferenciação por preço único (sem assinatura recorrente), API pública é diferencial técnico raro no setor, geração em volume (até 100 jogos no Ultimate) |
| Pontos fracos | Página principal (/produto) retornou erro 402 no fetch direto (indício de app SPA pago/paywall ou instabilidade); claims de IA não são auditáveis |
| UX/UI | Não confirmado em profundidade (SPA, difícil de auditar via fetch) |
| Presença digital | Blog ativo (posts sobre custo de apostas); Instagram não localizado na busca |
| Observações | É um dos concorrentes mais sofisticados encontrados em comunicação de produto (planos nomeados, API, "modelos" de IA nomeados) |

Fontes: [lotoai.com.br/planos](https://www.lotoai.com.br/planos), [lotoai.com.br/api-publica](https://www.lotoai.com.br/api-publica), [lotoai.com.br/pacotes](https://www.lotoai.com.br/pacotes)

---

### 2. Sortiq

| Campo | Detalhe |
|---|---|
| Produto | Sortiq |
| URL | https://sortiq.com.br/ |
| Plataforma | Web (SaaS) |
| Modalidades | Foco declarado em Mega-Sena (não confirmado se cobre todas as demais) |
| Público-alvo | Apostadores mais "técnicos", interessados em gestão financeira da aposta |
| Proposta principal | "Análise de Loterias com IA e Machine Learning" — posiciona-se como "parceiro inteligente na gestão de apostas" |
| Geração de jogos | Sim (simuladores) |
| IA | Comunica uso de Machine Learning + **Lei de Benford** + "momentum analysis" — combinação estatística real (Lei de Benford é uma técnica estatística legítima, ainda que sua aplicabilidade a sorteios aleatórios seja questionável), mas o site bloqueou fetch direto (403), então a real implementação não pôde ser auditada |
| Estatísticas | Sim (heatmaps) |
| Fechamentos | Não confirmado |
| Gestão de jogos | Sim — "dashboards financeiros" para planejar/validar/monitorar apostas; gestão de bolões mencionada |
| Conferência | Não confirmado |
| Automação com Caixa | Não encontrada evidência; dados "coletados da CEF" processados por algoritmos (fonte de dados, não automação de aposta) |
| Diferenciais | Enquadramento como ferramenta de "gestão financeira de apostas" (dashboard), não só gerador |
| Preço | Não confirmado (site bloqueou acesso automatizado) |
| Modelo de monetização | Provável SaaS/assinatura (não confirmado) |
| Pontos fortes | Posicionamento diferenciado (gestão + análise, não só geração aleatória) |
| Pontos fracos | Baixa transparência pública (bloqueio de scraping/fetch); presença digital não localizada |
| UX/UI | Não confirmado |
| Presença digital | Não localizada (Instagram/redes não encontrados na busca) |
| Observações | Concorrente conceitualmente mais próximo do "Jogos Bem Feitos" em termos de proposta (gestão + IA + dashboards), mas com presença digital muito mais fraca aparentemente |

Fonte: [sortiq.com.br](https://sortiq.com.br/) (busca indexada; fetch direto bloqueado com HTTP 403)

---

### 3. IA da Loteria

| Campo | Detalhe |
|---|---|
| Produto | IA da Loteria |
| URL | https://www.iadaloteria.com.br/ |
| Plataforma | Web |
| Modalidades | Lotofácil, Mega-Sena, Lotomania, Quina |
| Público-alvo | Do iniciante ao "profissional avançado" — declaram 5.000+ usuários ativos |
| Proposta principal | "Inteligência Artificial para Análise Estatística de Loterias" |
| Geração de jogos | Sim ("Geração Inteligente de Jogos") |
| IA | Comunicação explícita e extensa: "algoritmos avançados de IA", chatbot de IA embutido no produto para interação com o usuário, análises de sazonalidade por número |
| Estatísticas | Muito completo: frequência histórica, atraso (números não sorteados), sequências consecutivas, padrão por dia da semana, números primos, sequência de Fibonacci, gráficos interativos |
| Fechamentos | Não mencionado explicitamente |
| Gestão de jogos | Perfis individuais por número, alertas de novos sorteios |
| Conferência | Não confirmado |
| Automação com Caixa | Nenhuma evidência |
| Diferenciais | Chat de IA conversacional dentro do produto (mais próximo do conceito "Trevin"); disclaimer educacional próprio afirmando natureza não-preditiva |
| Preço | Grátis (acesso completo, segundo o site) + Premium Mensal R$ 29,90 (preço promocional citado como R$ 99) + Premium Anual R$ 99/ano (regular R$ 990) — **modelo de preços com forte uso de âncora promocional agressiva** |
| Modelo de monetização | Freemium + assinatura |
| Pontos fortes | Interface de chat IA (feature rara entre concorrentes); grande superfície de estatísticas; disclaimer transparente de que a ferramenta não é preditiva |
| Pontos fracos | Preços "de/por" muito exagerados (R$990→R$99) são um sinal clássico de tática de vendas questionável, o que pode gerar desconfiança |
| UX/UI | Aparenta ser um produto relativamente maduro (dashboards, autenticação social) |
| Presença digital | Não mensurada em detalhe |
| Observações | É o concorrente com posicionamento de "IA conversacional" mais próximo ao conceito do Trevin do Jogos Bem Feitos |

Fonte: [iadaloteria.com.br](https://www.iadaloteria.com.br/)

---

### 4. iaSorte

| Campo | Detalhe |
|---|---|
| Produto | iaSorte |
| URL | https://www.iasorte.com/ |
| Plataforma | Web |
| Modalidades | As 9 loterias da Caixa: Mega-Sena, Lotofácil, Quina, Lotomania, Dupla Sena, Timemania, Dia de Sorte, Super Sete, +Milionária — **cobertura completa igual à do Jogos Bem Feitos** |
| Público-alvo | De iniciantes a apostadores "sérios" que buscam ferramentas analíticas avançadas |
| Proposta principal | "Sorte é bom. Sorte com dados é melhor." — baseia-se em 25.000+ sorteios oficiais analisados |
| Geração de jogos | Sim, com **19 estratégias de geração via "IA"** distribuídas por plano (8 no Basic, +8 no Pro, +3 exclusivas no Premium, com criação de estratégia customizada) |
| IA | Comunicação de "IA" fortemente associada a "estratégias" nomeadas — mas a real natureza (modelo estatístico vs. IA generativa/preditiva) não é auditável externamente |
| Estatísticas | Frequência, atraso ("recency"), filtros inteligentes (par/ímpar, sequências, primos) |
| Fechamentos | Não explicitamente mencionado como "fechamento", mas há filtros combinatórios |
| Gestão de jogos | Sistema de gestão de bolões ("syndicate management") |
| Conferência | Sim — "verificação automatizada de sorteio" com retorno em 30 minutos |
| Automação com Caixa | Nenhuma evidência de preenchimento automático no site da Caixa |
| Diferenciais | Backtesting formal contra dados históricos (recurso mais raro); cotas diárias de análise por plano (mecanismo de monetização por uso) |
| Preço | Basic R$ 29,90/mês (30 análises/dia) · Pro R$ 59,90/mês (100 análises/dia + backtesting) · Premium R$ 99,90/mês (análises ilimitadas + customização total) — **sem contrato de fidelidade, segundo o site** |
| Modelo de monetização | Assinatura recorrente em 3 níveis (SaaS clássico) |
| Pontos fortes | Cobertura completa das 9 modalidades; estrutura de planos madura e bem segmentada; backtesting é um recurso tecnicamente sério |
| Pontos fracos | Preço mais alto do setor entre os "geradores IA" (R$99,90/mês no topo); "19 estratégias" pode ser apenas variações de filtros estatísticos com marketing de IA |
| UX/UI | Não confirmado em detalhe |
| Presença digital | Não mensurada |
| Observações | É, junto com iaSorte e Sortiq, um dos concorrentes com modelo de assinatura recorrente mais próximo de um verdadeiro SaaS — bom benchmark de precificação |

Fonte: [iasorte.com](https://www.iasorte.com/)

---

### 5. Robô da Loto

| Campo | Detalhe |
|---|---|
| Produto | Robô da Loto |
| URL | https://robodaloto.com.br/ (marketing: /marketing/) |
| Plataforma | Web, com venda via infoproduto (checkout PerfectPay) |
| Modalidades | Lotofácil, Mega-Sena, Quina |
| Público-alvo | Massa/leigo — linguagem de infoproduto/marketing agressivo |
| Proposta principal | "O sistema inteligente que analisa padrões e maximiza suas chances de ganhar nas loterias" |
| Geração de jogos | Sim (palpites sugeridos) |
| IA | **Alegações fortemente exageradas e questionáveis**: "redes neurais profundas treinadas com milhões de combinações históricas" e "**85% chance de vitória aumentada**" — essa é exatamente o tipo de claim de marketing enganoso que a tarefa pediu para escrutinar. Não há como uma rede neural aumentar a "chance de vitória" em um sorteio aleatório uniforme; isso é uma alegação estatisticamente indefensável |
| Estatísticas | Histórico de desempenho, monitoramento em tempo real |
| Fechamentos | Não confirmado |
| Gestão de jogos | Histórico de jogos |
| Conferência | Sim ("análise automática de resultados") |
| Automação com Caixa | Nenhuma evidência de preenchimento automático de apostas |
| Diferenciais | Notificações via WhatsApp, transmissões ao vivo dos sorteios |
| Preço | Não especificado no conteúdo público; checkout via PerfectPay (plataforma de infoprodutos/afiliados) |
| Modelo de monetização | Infoproduto digital com funil de vendas típico (provavelmente com programa de afiliados via PerfectPay) |
| Pontos fortes | Marketing agressivo capaz de gerar volume de tráfego (alega 15.000+ usuários) |
| Pontos fracos | Claims de "85% de chance" são altamente questionáveis e um risco de reputação para o setor como um todo; nota de rodapé "não afiliado à Caixa" sugere já ter recebido questionamentos |
| UX/UI | Página de vendas típica de infoproduto (não um dashboard de produto SaaS) |
| Presença digital | Não mensurada, mas modelo de negócio sugere tráfego pago/afiliados intenso |
| Observações | **Exemplo mais claro encontrado nesta pesquisa de "marketing de IA" sobre o que provavelmente é um gerador estatístico simples.** Útil como contraponto no posicionamento do Jogos Bem Feitos (ser tecnicamente honesto sobre o que a IA faz) |

Fonte: [robodaloto.com.br/marketing](https://robodaloto.com.br/marketing/)

---

### 6. Robô da Loteria

| Campo | Detalhe |
|---|---|
| Produto | Robô da Loteria |
| URL | https://robodaloteria.com.br/ |
| Plataforma | Web |
| Modalidades | Todas as 9 da Caixa + loterias alternativas (Lotinha, Super 6, Super 5) |
| Público-alvo | Jogadores em geral buscando praticidade |
| Proposta principal | "Geradores e jogos prontos" |
| Geração de jogos | Sim, geradores rápidos por modalidade |
| IA | Menção vaga a "sistema avançado", sem especificidade técnica |
| Estatísticas | Não aprofundado |
| Fechamentos | Não confirmado |
| Gestão de jogos | Não confirmado |
| Conferência | Não confirmado |
| Automação com Caixa | Nenhuma evidência |
| Diferenciais | Seção "Palpite do Dia" (em desenvolvimento); integra com plataformas parceiras de bolão/planilhas profissionais |
| Preço | Não especificado; parte dos serviços vinculada a "criar conta e ganhar bônus" em plataformas parceiras (sugere modelo de afiliados) |
| Modelo de monetização | Provável afiliados/parcerias |
| Pontos fortes | Cobertura ampla de modalidades, inclusive alternativas |
| Pontos fracos | Baixa profundidade de produto aparente; nome muito parecido com "Robô da Loto" pode gerar confusão de marca no mercado |
| UX/UI | Não confirmado |
| Presença digital | Não mensurada |
| Observações | — |

Fonte: [robodaloteria.com.br](https://robodaloteria.com.br/)

---

### 7. Joga Loterias Profissional (JLP)

| Campo | Detalhe |
|---|---|
| Produto | Joga Loterias Profissional |
| URL | https://www.jogaloterias.com.br/ |
| Plataforma | Web/Desktop + Extensão Chrome (JLP Apostas) |
| Modalidades | As 8-9 modalidades principais da Caixa (Mega-Sena, Quina, Dupla Sena, Lotofácil, Lotomania, Timemania, Dia de Sorte, Super Sete, +Milionária) |
| Público-alvo | Apostador "profissional"/frequente, disposto a pagar por ferramenta completa |
| Proposta principal | "O sistema definitivo para jogar loterias com inteligência" — trajetória de **15+ anos**, 159 versões lançadas, 440 artigos de blog |
| Geração de jogos | Sim, com "Categorias de Jogos divididos em Módulos" e geração de bolões |
| IA | Não usa terminologia de "IA" explícita — comunica como estatística/matemática tradicional |
| Estatísticas | Frequência, atraso, ciclos, desvio padrão em tempo real |
| Fechamentos | Sim — "pacotes matemáticos prontos" por loteria |
| Gestão de jogos | Sim (gerenciador interno do sistema, inclusive para distribuir a extensão) |
| Conferência | Sim (verificação e simulação de resultados) |
| **Automação com Caixa** | **Sim — via extensão "JLP Apostas"**, que preenche automaticamente múltiplas cartelas no site oficial da Caixa. **Achado crítico: a extensão foi removida/impedida na Chrome Web Store por violar as políticas de conteúdo de apostas/loteria, e desde a versão 2.9.5.600 passou a ser distribuída fora da loja, através do gerenciador interno do próprio software** |
| Diferenciais | Maior histórico/maturidade de produto entre os concorrentes desktop encontrados; integração vertical completa (análise → geração → fechamento → automação de preenchimento) |
| Preço | Não divulgado publicamente (checkout via "Comprar" sem valor exposto) |
| Modelo de monetização | Provável licença paga (assinatura ou vitalícia, não confirmado) |
| Pontos fortes | Produto mais completo e maduro entre os concorrentes desktop/legado; único com automação de preenchimento integrada de forma oficial ao produto principal |
| Pontos fracos | UX aparenta ser datada (produto desktop de origem antiga); distribuição fora da Chrome Web Store aumenta atrito de instalação (usuário precisa confiar em instalador manual/"developer mode") |
| UX/UI | Provavelmente datada — produto de origem desktop de 15+ anos |
| Presença digital | Blog extenso (440 artigos), mas presença em redes sociais não mensurada |
| Observações | **Este é o concorrente mais relevante para benchmarking direto da funcionalidade de automação de apostas do Jogos Bem Feitos.** É prova de mercado de que (a) existe demanda suficiente para automação de preenchimento de apostas, e (b) o Chrome Web Store efetivamente bloqueia esse tipo de extensão quando identificada, forçando distribuição alternativa |

Fontes: [jogaloterias.com.br](https://www.jogaloterias.com.br/), [jogaloterias.com.br/chrome-extensao-jlp-apostas](https://www.jogaloterias.com.br/chrome-extensao-jlp-apostas), [jogaloterias.com.br/atualizacoes](https://www.jogaloterias.com.br/atualizacoes)

---

### 8. LotoCarva

| Campo | Detalhe |
|---|---|
| Produto | LotoCarva |
| URL | https://lotocarva.com/ |
| Plataforma | Web |
| Modalidades | 10 loterias: Mega-Sena, Lotofácil, Quina, Lotomania, Dupla Sena, Timemania, Dia de Sorte, +Milionária, Super Sete, Loteca |
| Público-alvo | De iniciantes a apostadores estratégicos |
| Proposta principal | "413 fechamentos matemáticos exclusivos" |
| Geração de jogos | Sim, com desdobramentos matemáticos |
| IA | **Não comunica uso de IA** — se posiciona explicitamente em cima de matemática/estatística histórica, sem apelo a "inteligência artificial". É um contraponto interessante: prova que um concorrente relevante prefere não usar o termo "IA" |
| Estatísticas | Dezenas quentes/frias, ciclos |
| Fechamentos | Sim, extenso catálogo (413 fechamentos) — é provavelmente o maior catálogo de fechamentos prontos encontrado na pesquisa |
| Gestão de jogos | Recurso de "bolão comunitário" |
| Conferência | Sim — conferidor de bilhetes premiados |
| Automação com Caixa | Nenhuma evidência |
| Diferenciais | Simulador para testar estratégias contra histórico; ferramentas de cálculo (probabilidade, numerologia) |
| Preço | Teste gratuito de 7 dias; planos Semestral ou Anual (valores não divulgados publicamente) |
| Modelo de monetização | Freemium com trial + assinatura |
| Pontos fortes | Catálogo de fechamentos muito robusto; cobertura de 10 modalidades incluindo Loteca |
| Pontos fracos | Preços não transparentes publicamente (barreira de conversão) |
| UX/UI | Não confirmado em detalhe |
| Presença digital | Não mensurada |
| Observações | — |

Fonte: [lotocarva.com](https://lotocarva.com/gerador-de-jogos-gratis/mega-sena)

---

### 9. Mega Fácil

| Campo | Detalhe |
|---|---|
| Produto | Mega Fácil (megafacil.app) |
| URL | https://www.megafacil.app/ |
| Plataforma | Web + app mobile integrado |
| Modalidades | 12 loterias: Mega-Sena, Quina, Dupla-Sena, Loteca, Lotofácil, Lotomania, Lotogol, Timemania, Federal, Dia de Sorte, Super Sete, +Milionária — **cobertura mais ampla que a maioria dos concorrentes** |
| Público-alvo | Amplo, de iniciante a frequente |
| Proposta principal | Conveniência: gerador + estatística + conferência automática integrados |
| Geração de jogos | Sim (aleatório ou "seleção automática") |
| IA | Não comunicado explicitamente |
| Estatísticas | Frequências e padrões históricos |
| Fechamentos | Sim (sistemas de combinações matemáticas) |
| Gestão de jogos | Não aprofundado |
| Conferência | Sim, validação automática de bilhetes contra resultados |
| Automação com Caixa | Nenhuma evidência |
| Diferenciais | Gratuidade total do produto (monetização não é via assinatura de features) |
| Preço | Gratuito |
| Modelo de monetização | Provavelmente ads/afiliados (apostas via Caixa a partir de R$3,50 citadas no conteúdo, sugerindo modelo de conteúdo/tráfego, não SaaS) |
| Pontos fortes | Gratuito, cobertura ampla de modalidades |
| Pontos fracos | Sem diferenciação por IA/tecnologia — concorre por volume/gratuidade, não por sofisticação |
| UX/UI | Não confirmado |
| Presença digital | Não mensurada |
| Observações | — |

Fonte: [megafacil.app/gerador/megasena](https://www.megafacil.app/gerador/megasena)

---

### 10. JOGO FÁCIL Profissional (softdeloteria.com.br)

| Campo | Detalhe |
|---|---|
| Produto | JOGO FÁCIL Profissional |
| URL | https://softdeloteria.com.br/ |
| Plataforma | Desktop (Windows, provável) |
| Modalidades | Mega-Sena, Lotofácil, Lotomania, Quina, Dupla Sena, Timemania, Dia de Sorte, Super Sete |
| Público-alvo | Apostador "profissional"/entusiasta de longa data, tolerante a software desktop tradicional |
| Proposta principal | Software de 15 anos para "criar, analisar e organizar jogos com mais agilidade" |
| Geração de jogos | Sim — "Gerador de Matrizes ilimitado", comparado a ferramentas internacionais como ININUGA e COVERMASTER |
| IA | Não comunicado |
| Estatísticas | Sim (análise estatística) |
| Fechamentos | Sim (fechamentos matemáticos, com suporte a "redutor de jogos") |
| Gestão de jogos | Sim |
| Conferência | Não confirmado |
| Automação com Caixa | **Sistema de impressão que configura e imprime jogos diretamente no formato do boletim oficial da Caixa** — não é preenchimento automático no site, mas impressão formatada para uso físico/manual |
| Diferenciais | Licença vitalícia de baixo custo; comparação direta com softwares internacionais de "wheeling" (fechamento) |
| Preço | **R$ 110,00, licença vitalícia** |
| Modelo de monetização | Compra única |
| Pontos fortes | Preço muito baixo para acesso vitalício; 15 anos de mercado sugerem base de usuários fiel |
| Pontos fracos | Site com aparência datada (Joomla, "sample-data-articles" nas URLs — indício de site desatualizado tecnicamente); só desktop, sem mobile/web moderno |
| UX/UI | Provavelmente datada (site institucional em Joomla) |
| Presença digital | Fraca aparentemente |
| Observações | Representa o segmento "legado" do mercado — usuários antigos de software de fechamento que nunca migraram para SaaS |

Fonte: [softdeloteria.com.br](https://softdeloteria.com.br/)

---

### 11. LoteriaSoft (netsorte.com)

| Campo | Detalhe |
|---|---|
| Produto | LoteriaSoft / Programa LoteriaSoft |
| URL | https://netsorte.com/programa-loteriasoft/fechamento-loterico/ |
| Plataforma | Desktop |
| Modalidades | Múltiplas, incluindo Loteca |
| Público-alvo | Apostador avançado/técnico |
| Proposta principal | "O Melhor Software de Loteria da Internet Brasileira" |
| Geração de jogos | Sim, com importação de combinações próprias |
| IA | Não comunicado |
| Estatísticas | Não aprofundado |
| Fechamentos | Sim — com filtros avançados (pares, ímpares, bordas, meios, primos) aplicáveis aos fechamentos |
| Gestão de jogos | Painel de ferramentas para importar jogos/combinações |
| Conferência | Não confirmado |
| Automação com Caixa | Nenhuma evidência |
| Diferenciais | Filtros de fechamento granulares (nível de sofisticação técnica alto para o segmento) |
| Preço | Não confirmado |
| Modelo de monetização | Não confirmado (provavelmente venda de licença) |
| Pontos fortes | Sofisticação de filtros matemáticos |
| Pontos fracos | Site aparenta baixa qualidade de produção; Reclame Aqui tem página de reclamações registrada para "LoteriaSoft" (não foi possível auditar o teor específico) |
| UX/UI | Não confirmado |
| Presença digital | Possui página no Reclame Aqui (sinal de volume de usuários, positivo ou negativo não determinado) |
| Observações | Existe registro em https://www.reclameaqui.com.br/empresa/loteriasoft/lista-reclamacoes/ — recomenda-se auditoria futura direta se necessário |

Fonte: [netsorte.com/programa-loteriasoft](https://netsorte.com/programa-loteriasoft/fechamento-loterico/)

---

### 12. Apps mobile "geradores IA" (App Store / Google Play) — cauda longa

Esta categoria é extremamente fragmentada. Resumo consolidado dos achados mais relevantes:

| App | Loja | Preço | IA? | Avaliação | Observação |
|---|---|---|---|---|---|
| **Gera-Loteca** | iOS | Free + assinatura Premium R$9,90/mês | Sim, modo IA + modo aleatório + gerador de bolão | **4,8★ / 98 avaliações** | Melhor avaliação encontrada no segmento; reclamação recorrente: excesso de anúncios |
| **LOTERIA AI** | iOS/Android | US$2,99/mês ou US$17,99/ano | Sim — "IA" com 4 estratégias: Números Quentes, Frios, Mix Inteligente, 100% Aleatório | Não confirmado (avaliações não localizadas) | Alega 30 anos de dados da Mega-Sena e 20+ da Lotofácil, "100% dados oficiais Caixa" |
| **IA DA LOTOFACIL – Análise IA** | Android (com.matrix.lotofacil) | Não confirmado | Sim — alega 29 anos de dados públicos | Reclamações associadas a produtos similares relatam "dicas aleatórias sem fundamento" | Disclaimer próprio: "não faz apostas, não registra jogos" — só ferramenta de estudo |
| **Visão Lotofácil / Visão Mega-Sena** (dzdev) | Android | Não confirmado | Não destaca IA explicitamente | Não confirmado | Foco em portfólio de jogos + estatística visual |
| **Loterias Mais Fácil** | Android (com.kacyano.megasena) | Gratuito | Não confirmado | Reclamações de bug (resultados travados em ano 2000 ao desligar WiFi, supostamente corrigido) | Módulo "D.Sorte" para loterias alternativas com até 21 dezenas |
| **fácil Number Generator** | Android (com.mountain.lotofacil) | Gratuito | Não | Não confirmado | Disclaimer explícito de não ter relação com órgão governamental |
| Cauda longa adicional identificada | Android | Majoritariamente gratuitos | Raramente | Não confirmado | "Gerador Lotofacil Advanced", "LiteLoto Generator Lotofacil", "Gerador Lotofácil" (XErikProductions), "Lotofácil - Gerador de Números" (impera), "Gerador de Números Loto Fácil" — dezenas de apps de baixíssima diferenciação, provavelmente feitos por desenvolvedores individuais/indie |

**Observação geral sobre a categoria mobile**: o mercado de apps de loja é extremamente pulverizado — dezenas de aplicativos praticamente idênticos (gerador aleatório com filtro básico), a maioria sem marca forte, sem suporte visível e sem real diferenciação por IA, mesmo quando usam o termo no nome/descrição.

Fontes: [Gera-Loteca](https://apps.apple.com/br/app/gera-loteca/id6466176647), [LOTERIA AI](https://apps.apple.com/in/app/loteria-ai/id6758863169), [IA DA LOTOFACIL](https://play.google.com/store/apps/details?id=com.matrix.lotofacil), [Loterias Mais Fácil](https://play.google.com/store/apps/details?id=com.kacyano.megasena), [fácil Number Generator](https://play.google.com/store/apps/details?id=com.mountain.lotofacil)

---

### 13. Produtos com forte sinal de golpe/propaganda enganosa (relevante para benchmarking de risco reputacional do setor)

| Produto | Evidência |
|---|---|
| **Loto Lógica** | Mais de **300 relatos de golpe no Reclame Aqui**; matéria de fact-check da Agência Lupa (24/09/2025) classificando-a como golpe: "É golpe aplicativo que promete acertar números para ganhar na Loteria". Um usuário relatou: "descobri que não existe sistema, apenas tendo que jogar a loteria através do site deles. Um site que nem sequer é autorizado para realizar esse tipo de jogo de azar." A Caixa afirmou publicamente que "não há brechas ou falhas nos sistemas da Loteria que permitam prever ou influenciar os números sorteados" |
| **Loto Sniper** | Reclamação no Reclame Aqui intitulada "Não compre esse programa - TUDO MENTIRA E POSSO PROVAR" |
| **Gênio da Lotofácil** | Múltiplas reclamações via processadores de pagamento (Voluti Pagamentos, PerfectPay) |
| **Sistema "Lotofácil com IA" via Cakto Pay** | Reclamação: "Propaganda enganosa de sistema de apostas Lotofácil com IA e dificuldade de contato para reembolso" |
| Padrão geral identificado | Um gerador de números "sem metodologia" tende a acertar 7-9 dezenas na Lotofácil por acaso estatístico — o que não gera prêmio, mas é usado por produtos duvidosos como "prova" de eficácia em marketing |

Fontes: [Agência Lupa](https://www.agencialupa.org/jornalismo/2025/09/25/e-golpe-aplicativo-que-promete-acertar-numeros-para-ganhar-na-loteria/), [Reclame Aqui - Loto Lógica](https://www.reclameaqui.com.br/empresa/loto-logica/lista-reclamacoes/), [Reclame Aqui - Loto Sniper](https://www.reclameaqui.com.br/loto-sniper/nao-compre-esse-programa-tudo-mentira-e-posso-provar_RPre3cuGBWepQFzN/)

**Implicação estratégica**: este é um mercado com histórico documentado de golpes e propaganda enganosa envolvendo justamente o termo "IA" aplicado a loteria. Isso é uma faca de dois gumes para o Jogos Bem Feitos — de um lado, ceticismo do consumidor pré-instalado contra "IA + loteria"; de outro, uma oportunidade de diferenciação por transparência e honestidade sobre o que a ferramenta realmente faz (organização/gestão, não "previsão").

---

## PARTE 2 — CONCORRENTES INDIRETOS / ADJACENTES

### 14. Loterias CAIXA (app oficial)

| Campo | Detalhe |
|---|---|
| URL | https://www.caixa.gov.br/atendimento/aplicativos/app-loterias/ · https://play.google.com/store/apps/details?id=br.gov.caixa.loterias.apostas |
| Plataforma | Android, iOS, Web |
| Modalidades | Todas (Mega-Sena, Lotofácil, Loteca, Dia de Sorte, +Milionária, Quina, Timemania, Super Sete, Dupla Sena, Lotogol, Federal) |
| Proposta principal | App oficial de apostas — permite Surpresinha, Teimosinha, Bolão CAIXA, histórico de apostas, conferência de resultados, leitura de código de barras de bilhetes físicos |
| Geração de jogos | Sim, mas apenas "completar com números aleatórios" (não é gerador estatístico) |
| Automação/Bolão | **Recurso de bolão oficial**: usuários compram cotas de grupos organizados por lotéricas, pagamento individual via Pix/cartão, recibo digital vinculado ao CPF. Esse recurso reduz a necessidade de ferramentas terceiras de organização de bolão para o caso de uso mais simples |
| Preço | Gratuito (paga-se apenas a aposta) |
| Pontos fortes | Confiabilidade máxima (é o canal oficial), inclui bolão nativo |
| Pontos fracos | UX considerada básica pelos concorrentes (não tem estatística avançada, geração inteligente, fechamento) — é exatamente o vácuo que os concorrentes exploram |
| Observações | É o "chão" competitivo — qualquer ferramenta precisa ser comparada com o que o app oficial já entrega de graça |

Fontes: [caixa.gov.br/app-loterias](https://www.caixa.gov.br/atendimento/aplicativos/app-loterias/Paginas/default.aspx), [Olhar Digital sobre bolão no app Caixa](https://olhardigital.com.br/curiosidades/2026/05/24/o-recurso-escondido-no-aplicativo-da-caixa-que-facilita-a-vida-de-quem-quer-jogar-em-grupo/)

---

### 15. Intersena

| Campo | Detalhe |
|---|---|
| URL | https://www.intersena.com.br/ |
| Plataforma | Web |
| Proposta principal | "1º Portal de Loterias Online do Brasil" — **26 anos de atuação**, revendedor autorizado operando via lotéricas credenciadas pela Caixa |
| Modalidades | As 9 principais |
| Funcionalidades | Fechamento com análise matemática, simulador de sorte, compra de bilhetes em grupo (bolão) via Pix/cartão/boleto |
| Preço | A partir de R$ 4,50/bilhete (Lotofácil 15 números) |
| Confiabilidade | Reclame Aqui mostra avaliações majoritariamente positivas; reclamação antiga (2018) sobre recebimento de prêmio, já fora do índice atual |
| Pontos fortes | Marca legada e confiável (26 anos), modelo de revenda autorizada dá segurança jurídica |
| Observações | Representa o segmento de "loterias online revendedoras" — adjacente porque compete pela atenção do apostador de bolão/fechamento, mas não é gerador de jogos com IA |

Fontes: [intersena.com.br](https://www.intersena.com.br/), [Reclame Aqui - Intersena](https://www.reclameaqui.com.br/empresa/intersena/)

---

### 16. Conferir Acertos na Loteria (app)

| Campo | Detalhe |
|---|---|
| URL | https://play.google.com/store/apps/details?id=br.com.estudiowebapps.cal |
| Plataforma | Android |
| Proposta principal | App simples e independente de conferência de jogos registrados manualmente (não faz apostas) |
| Preço | Não confirmado (provavelmente gratuito/ads) |
| Diferencial | Disclaimer explícito: "independente, sem conexão com a Caixa ou qualquer entidade governamental" |
| Observações | Exemplo do segmento "utilitário de conferência" — baixa sofisticação, alto volume potencial de usuários (necessidade recorrente e simples) |

Fonte: [Play Store - Conferir Acertos](https://play.google.com/store/apps/details?id=br.com.estudiowebapps.cal)

---

### 17. Loterias: Resultados e Gerador

| Campo | Detalhe |
|---|---|
| URL | https://apps.apple.com/br/app/loterias-resultados-e-gerador/id6478125067 |
| Plataforma | iOS (também há versão Android por outros devs com nome similar) |
| Preço | Premium Mensal R$ 4,90 |
| Observações | App combinando resultados oficiais + gerador básico — representa o segmento "app utilitário de resultados com upsell de gerador" |

Fonte: busca App Store

---

### 18. Bolão APP / Bolão Entre Amigos / Bolaoja (gestão de bolões)

| Campo | Detalhe |
|---|---|
| URLs | https://www.obolaoapp.com.br/ · https://apps.apple.com/br/app/bol%C3%A3o-entre-amigos/id6446399984 |
| Plataforma | Android/iOS |
| Preço | Bolão APP: gratuito |
| Observações importante | **A maior parte dos resultados de busca para "Bolão App" refere-se a bolões de futebol (Copa do Mundo, campeonatos), não a bolões de loteria da Caixa.** É um adjacente relevante apenas como benchmark de UX de "gestão de grupo/rateio", não como concorrente direto de produto |

Fonte: busca combinada App Store/Google Play

---

### 19. XLOTO Gestão

| Campo | Detalhe |
|---|---|
| URL | https://xloto.com.br/ |
| Plataforma | Web/mobile |
| Proposta principal | Software de gestão B2B para **lotéricas** (donos de casas lotéricas), não para apostadores finais |
| Funcionalidades | Fechamento automatizado de caixa com conexão à CEF, controle de conta 043, 43+ análises gerenciais, gestão de bolões e cotas via WhatsApp |
| Preço | A partir de R$ 180,00/mês |
| Público-alvo | 1.200+ lotéricas clientes, segundo o site |
| Observações | Adjacente relevante porque mostra que existe todo um ecossistema B2B de "gestão de bolão via WhatsApp" operado pelas próprias lotéricas — um canal de distribuição/parceria potencial, mas também um concorrente indireto pela atenção do "gestor de bolão" |

Fonte: [xloto.com.br](https://xloto.com.br/)

---

### 20. Só Matemática — Simulador da Lotofácil

| Campo | Detalhe |
|---|---|
| URL | https://www.somatematica.com.br/lotofacil.php |
| Plataforma | Web |
| Proposta principal | Ferramenta educacional gratuita, gerador + teste de números contra concursos anteriores, conteúdo sobre desdobramentos/fechamentos |
| Observações | Domínio educacional antigo e de alto tráfego orgânico (SEO) — concorre por atenção/busca orgânica (ex: "fechamento lotofácil"), não por produto sofisticado. Relevante para estratégia de SEO/conteúdo do Jogos Bem Feitos |

Fonte: [somatematica.com.br/lotofacil.php](https://www.somatematica.com.br/lotofacil.php)

---

### 21. Comunidade Reclame Aqui / YouTube (canais de "exposição de golpe")

| Campo | Detalhe |
|---|---|
| Observação | Existe uma comunidade ativa de conteúdo em YouTube dedicada a expor golpes de loteria com IA (ex.: "Golpe do APP Loto Lógica - Falsa promessa de 14 pontos Lotofácil", "Golpe do APP Loto Lógica - Fraude Comprovada"), além do Reclame Aqui funcionando como canal de denúncia coletiva |
| Relevância | Formadores de opinião/"watchdogs" que podem afetar a percepção pública de qualquer ferramenta de loteria que use o termo IA — o Jogos Bem Feitos deve estar preparado para esse escrutínio |

Fonte: busca YouTube/Reclame Aqui

---

## AUTOMAÇÃO COM A CAIXA — ANÁLISE ESPECÍFICA

### Quem faz isso hoje

Identificamos **6 soluções ativas ou historicamente ativas** de automação de preenchimento de apostas no site oficial `loteriasonline.caixa.gov.br`:

| Solução | Distribuição | Status | Usuários/tração | Open source |
|---|---|---|---|---|
| **Apostas automáticas Loterias Caixa** (dev. Jonathan Ferreira Silva) | Chrome Web Store | Ativa (última atualização set/2023) | 770 usuários, 3,7★ (12 avaliações) | Não |
| **Automação Loterias Caixa** (dev. Bruno Siqueira Ferreira) | Chrome Web Store | Ativa e **recentemente atualizada (jan/2026)** | 123 usuários, sem avaliações | Não |
| **ChromeLoteca** (LukeC8) | GitHub (instalação manual/"modo desenvolvedor") | Ativa, open source | 9 estrelas / 8 forks no GitHub | Sim, GPLv3 |
| **INJOLOCA** (guynovaes) | GitHub (instalação manual) | Ativa, open source | 21 estrelas / 14 forks no GitHub | Sim, GPLv3 |
| **JLP Apostas** (Joga Loterias Profissional) | **Removida da Chrome Web Store**; distribuída via gerenciador interno do software pago desde a v2.9.5.600 | Ativa, mas fora da loja oficial | Não divulgado (parte de produto pago maior) | Não |
| **LotoSport** | Arquivo de instalação manual (fora da Chrome Web Store) | Ativa | Não confirmado | Não confirmado |

### Como funciona tecnicamente

Todas as soluções seguem o mesmo padrão básico:
1. O usuário cola/importa uma lista de jogos (números separados por vírgula, espaço, ponto-e-vírgula ou traço, geralmente vindos de um arquivo texto ou de um gerador/fechamento externo).
2. A extensão manipula o DOM da página `loteriasonline.caixa.gov.br` (não usa API oficial da Caixa — não existe API pública de apostas), simulando cliques e preenchendo os campos de número automaticamente.
3. O usuário revisa e confirma manualmente a finalização da compra no carrinho — nenhuma das soluções encontradas afirma automatizar o pagamento/checkout final, apenas o preenchimento.
4. As permissões declaradas se restringem ao domínio `loteriasonline.caixa.gov.br` (segundo a documentação do ChromeLoteca), e os desenvolvedores fazem questão de declarar publicamente que "não coletam login/senha" — um sinal de que a confiança/segurança é uma objeção recorrente do usuário nesse nicho.

### Quanto custa

- As duas extensões atualmente na Chrome Web Store são **gratuitas** com "compras no app" (modelo freemium, provavelmente limite de jogos/cartelas grátis e desbloqueio pago para volume maior — não confirmado o valor exato).
- ChromeLoteca e INJOLOCA são **gratuitos e open source** (GPLv3).
- JLP Apostas é **gratuita apenas para quem já é cliente pago** do software Joga Loterias Profissional (preço do software principal não divulgado publicamente).

### É demanda relevante? Evidências

Sim, há evidências consistentes de demanda:
- **Múltiplas soluções independentes e concorrentes entre si** resolvendo exatamente o mesmo problema (preenchimento manual de apostas), incluindo pelo menos 2 projetos open source mantidos por desenvolvedores voluntários sem monetização aparente — sinal forte de "dor" real o suficiente para alguém construir de graça.
- Comunicação de marketing recorrente em todas as soluções: "evite perder tempo preenchendo bilhete por bilhete", "ideal para quem aposta com desdobramentos e fechamentos", "o portal oficial não permite envio em lote" — este último ponto (JLP) é uma confirmação direta de que **a Caixa não oferece nativamente um mecanismo de importação em lote**, o que é a lacuna que toda essa categoria de produto explora.
- A funcionalidade é claramente pensada para o público que já usa fechamento/desdobramento (jogos com 16+ números geram múltiplas cartelas de 15 números na Lotofácil, por exemplo) — ou seja, a automação de preenchimento é o "último passo" natural de qualquer ferramenta de geração/fechamento, o que valida a arquitetura de produto do Jogos Bem Feitos (gerar + organizar + preencher).
- Não foi encontrada, na pesquisa, nenhuma reclamação pública massiva no Reclame Aqui especificamente sobre "dificuldade de preencher manualmente" (é uma dor operacional, não uma queixa formal), mas a proliferação de soluções é evidência indireta forte.

### Riscos técnicos e jurídicos

**1. Risco de banimento na Chrome Web Store — já materializado no mercado.**
A pesquisa confirmou dois fatos centrais:
- A Chrome Web Store possui política explícita ("Regulated goods and services") que **não permite conteúdo ou serviços que facilitem ou promovam jogos de azar (gambling) com dinheiro real, incluindo loterias**, segundo a documentação oficial do Google ([developer.chrome.com/docs/webstore/program-policies/regulated-goods-and-services](https://developer.chrome.com/docs/webstore/program-policies/regulated-goods-and-services)).
- **A extensão JLP Apostas foi de fato barrada/removida da Chrome Web Store por essa política e precisou migrar para distribuição via instalador manual** — este é o caso documentado mais direto de enforcement dessa política contra uma ferramenta do nicho de loteria brasileira.
- Ao mesmo tempo, duas outras extensões (Jonathan Ferreira Silva e Bruno Siqueira Ferreira) **seguem ativas na loja até hoje**, uma delas com atualização recente (janeiro de 2026) — o que sugere enforcement inconsistente/reativo por parte do Google, não uma varredura proativa e sistemática. Isso significa que uma extensão pode operar por anos sem problema até ser denunciada/revisada e então removida sem aviso, o que é um risco de continuidade de produto real para qualquer negócio que dependa dela como canal principal.

**2. Risco quanto aos Termos de Uso da Caixa.**
Não foi possível auditar diretamente o texto completo dos Termos de Uso do `loteriasonline.caixa.gov.br` (página renderizada via JavaScript/SPA, inacessível a fetch automatizado — **não confirmado o teor exato**). Como padrão de mercado, sites de terceiros que revendem apostas da Caixa (ex.: LotoLoterias) declaram explicitamente em seus próprios termos: *"É proibido usar bots ou scripts automatizados para explorar o site, tentar violar sistemas de segurança e copiar ou redistribuir conteúdo sem permissão"* — uma cláusula padrão do setor que muito provavelmente also existe (não confirmado literalmente) nos termos da própria Caixa, já que é prática comum em portais .gov.br e de instituições financeiras. Nenhuma das extensões auditadas apresenta ao usuário um aviso legal sobre esse risco de violação de termos de uso — o que é uma lacuna de compliance generalizada no setor, não só de um concorrente específico.

**3. Risco de segurança/confiança do usuário.**
Como a extensão precisa operar sobre a sessão autenticada do usuário no site da Caixa (mesmo sem capturar login/senha diretamente, segundo alegam os desenvolvedores), há um risco reputacional inerente: qualquer falha, bug ou ação maliciosa de uma extensão de terceiros rodando sobre um site financeiro gera desconfiança de fraude. Os próprios desenvolvedores tentam mitigar isso destacando publicamente "não coletamos dados de login" — uma prova de que essa é a principal objeção do público-alvo.

**4. Risco de descontinuação técnica unilateral pela Caixa.**
Como as extensões dependem de manipulação de DOM (não de API oficial), qualquer mudança de layout/estrutura do site `loteriasonline.caixa.gov.br` pode quebrar a automação sem aviso prévio — um risco técnico de manutenção contínua, não jurídico.

### Implicação estratégica para o Jogos Bem Feitos

A automação de preenchimento é claramente uma funcionalidade validada por mercado (múltiplos concorrentes, inclusive open source, resolvendo o mesmo problema), mas **nenhum concorrente parece ter resolvido de forma robusta e sustentável o problema de distribuição via Chrome Web Store** — o caso da JLP (removida e forçada a distribuir fora da loja) é o precedente mais direto e deveria ser tratado como um risco operacional real a ser mitigado (ex.: arquitetura que minimize a superfície de política violada, comunicação cuidadosa na ficha da extensão, ou plano de contingência de distribuição alternativa caso a extensão do Jogos Bem Feitos seja removida).

---

## FONTES CONSOLIDADAS

- [LotoAI](https://www.lotoai.com.br/) — [planos](https://www.lotoai.com.br/planos) — [API](https://www.lotoai.com.br/api-publica) — [pacotes](https://www.lotoai.com.br/pacotes)
- [Sortiq](https://sortiq.com.br/)
- [IA da Loteria](https://www.iadaloteria.com.br/)
- [iaSorte](https://www.iasorte.com/)
- [Robô da Loto](https://robodaloto.com.br/marketing/)
- [Robô da Loteria](https://robodaloteria.com.br/)
- [Joga Loterias Profissional](https://www.jogaloterias.com.br/) — [Extensão JLP](https://www.jogaloterias.com.br/chrome-extensao-jlp-apostas) — [Atualizações](https://www.jogaloterias.com.br/atualizacoes)
- [LotoCarva](https://lotocarva.com/gerador-de-jogos-gratis/mega-sena)
- [Mega Fácil](https://www.megafacil.app/gerador/megasena)
- [JOGO FÁCIL Profissional](https://softdeloteria.com.br/)
- [LoteriaSoft / Netsorte](https://netsorte.com/programa-loteriasoft/fechamento-loterico/)
- [Lotowise](https://www.lotowise.com.br/)
- [Lotofácil Inteligente](https://lotofacilinteligente.com.br/)
- [Gera-Loteca (App Store)](https://apps.apple.com/br/app/gera-loteca/id6466176647)
- [LOTERIA AI (App Store)](https://apps.apple.com/in/app/loteria-ai/id6758863169)
- [IA DA LOTOFACIL (Google Play)](https://play.google.com/store/apps/details?id=com.matrix.lotofacil)
- [Loterias Mais Fácil (Google Play)](https://play.google.com/store/apps/details?id=com.kacyano.megasena)
- [fácil Number Generator (Google Play)](https://play.google.com/store/apps/details?id=com.mountain.lotofacil)
- [Apostas automáticas Loterias Caixa (Chrome Web Store)](https://chromewebstore.google.com/detail/apostas-autom%C3%A1ticas-loter/lleccpmgmkoajogkgmnpbgoodgebpnlb)
- [Automação Loterias Caixa (Chrome Web Store)](https://chromewebstore.google.com/detail/automa%C3%A7%C3%A3o-loterias-caixa/ndlbkaamjcndgcjhhcbneeignadioohf)
- [ChromeLoteca (GitHub)](https://github.com/LukeC8/chromeloteca)
- [INJOLOCA (GitHub)](https://github.com/guynovaes/INJOLOCA)
- [Chrome Web Store - Regulated Goods and Services Policy](https://developer.chrome.com/docs/webstore/program-policies/regulated-goods-and-services)
- [Loterias CAIXA — app oficial](https://www.caixa.gov.br/atendimento/aplicativos/app-loterias/Paginas/default.aspx)
- [Olhar Digital — bolão no app da Caixa](https://olhardigital.com.br/curiosidades/2026/05/24/o-recurso-escondido-no-aplicativo-da-caixa-que-facilita-a-vida-de-quem-quer-jogar-em-grupo/)
- [Intersena](https://www.intersena.com.br/)
- [Conferir Acertos na Loteria (Google Play)](https://play.google.com/store/apps/details?id=br.com.estudiowebapps.cal)
- [XLOTO Gestão](https://xloto.com.br/)
- [Só Matemática — Simulador Lotofácil](https://www.somatematica.com.br/lotofacil.php)
- [Agência Lupa — "É golpe aplicativo que promete acertar números"](https://www.agencialupa.org/jornalismo/2025/09/25/e-golpe-aplicativo-que-promete-acertar-numeros-para-ganhar-na-loteria/)
- [Reclame Aqui — Loto Lógica](https://www.reclameaqui.com.br/empresa/loto-logica/lista-reclamacoes/)
- [Reclame Aqui — Loto Sniper](https://www.reclameaqui.com.br/loto-sniper/nao-compre-esse-programa-tudo-mentira-e-posso-provar_RPre3cuGBWepQFzN/)
- [Reclame Aqui — LoteriaSoft](https://www.reclameaqui.com.br/empresa/loteriasoft/lista-reclamacoes/)
- [Reclame Aqui — Cakto Pay (sistema Lotofácil IA)](https://www.reclameaqui.com.br/cakto-pay/propaganda-enganosa-de-sistema-de-apostas-lotofacil-com-ia-e-dificuldade-de_SAkNrLzty_WI0Zni/)

---

## LIMITAÇÕES DA PESQUISA (transparência metodológica)

- Vários sites usam frameworks JS/SPA que bloqueiam extração de conteúdo via fetch automatizado (LotoAI /produto, Sortiq, Lotowise, Lotofácil Inteligente, termos de uso do site oficial da Caixa) — nesses casos os dados vêm de resultados de busca indexados, não de leitura direta da página, e estão marcados como tal.
- Não foi possível confirmar números exatos de instalação/faturamento para a maioria dos produtos — quase nenhum divulga isso publicamente.
- O texto literal dos Termos de Uso do site `loteriasonline.caixa.gov.br` sobre proibição de automação **não foi confirmado** diretamente (página inacessível a scraping); a inferência sobre essa cláusula existir é baseada em padrão consistente encontrado em revendedores autorizados terceiros, não é uma citação direta da Caixa.
- Não há acesso direto às lojas de app (App Store/Google Play) além de dados indexados por busca — números de instalação exibidos na loja (quando existentes) não puderam ser todos confirmados com precisão.
