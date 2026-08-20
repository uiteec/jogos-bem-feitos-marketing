# Pesquisa de Mercado: Comportamento e Dores de Apostadores de Loterias Caixa
### Base para análise de Jobs To Be Done — Jogos Bem Feitos

**Nota metodológica honesta:** a pesquisa foi feita via busca web (WebSearch) e tentativas de acesso direto a páginas (WebFetch). Reclame Aqui bloqueou acesso direto ao conteúdo completo (HTTP 403) na maioria das tentativas — as evidências dessa fonte vêm dos *snippets/resumos* retornados pela busca, não da leitura integral das páginas, e isso está marcado explicitamente abaixo. Buscas diretas por "site:reddit.com" não retornaram resultados do Reddit relevantes (o Reddit parece pouco indexado/pouco usado para esse nicho em português, ou a busca não teve acesso a esse conteúdo) — não encontrei evidência substancial de discussões no Reddit brasileiro sobre o tema, e isso é registrado como lacuna, não preenchido com invenção. Google Play e Chrome Web Store também limitaram o acesso a texto de reviews individuais na maioria dos casos (conteúdo truncado ou não exposto pela ferramenta de fetch) — os dados quantitativos (nota, nº de instalações) foram capturados quando disponíveis.

---

## 1. Dores por Categoria (com evidências)

### 1.1 Inserção/preenchimento manual de apostas no site da Caixa
Esta é a dor mais diretamente validada e é a que já gerou um mercado de extensões de terceiros — evidência forte de que "preencher jogos manualmente" é doloroso o suficiente para as pessoas instalarem extensões não oficiais.

- Existem pelo menos **4-5 extensões Chrome concorrentes** dedicadas só a isso: "Apostas automáticas Loterias Caixa" (chromewebstore.google.com/detail/lleccpmgmkoajogkgmnpbgoodgebpnlb), "Automação Loterias Caixa" (ndlbkaamjcndgcjhhcbneeignadioohf), "ChromeLoteca" (GitHub: LukeC8/chromeloteca), "INJOLOCA" (GitHub: guynovaes/INJOLOCA), e "JLP Apostas" (jogaloterias.com.br). O simples fato de existirem múltiplas extensões, algumas open-source feitas por desenvolvedores individuais sem fins comerciais claros, é evidência de que a dor é real e generalizada o bastante para motivar até soluções não-monetizadas.
- Texto de marketing da extensão líder (770 instalações, nota 3.7/5, 12 avaliações — dados capturados via fetch direto do Chrome Web Store): *"Crie seu bolão e deixa que a gente faça o trabalho difícil de preencher os bilhetes!"* — a própria copy do concorrente nomeia o preenchimento como "trabalho difícil" (`chromewebstore.google.com/detail/apostas-automáticas-loter/lleccpmgmkoajogkgmnpbgoodgebpnlb`).
- A extensão ChromeLoteca e a INJOLOCA fazem questão de deixar claro que **não pedem login/senha e não coletam dados** — isso sinaliza (por precaução defensiva do próprio desenvolvedor) que confiança/segurança é uma objeção central que os usuários levantam antes de instalar algo que mexe no site da Caixa.
- Nota 3.7/5 com apenas 12 avaliações sugere um produto que resolve a dor mas de forma mediana — não é um "uau", é um "alívio parcial". Não há texto de review individual disponível para citar diretamente (limitação da ferramenta).

### 1.2 Instabilidade e lentidão do site/app oficial da Caixa
Fonte robusta: TechTudo e múltiplos títulos de reclamações no Reclame Aqui (via snippets de busca).

- TechTudo (dez/2024): *"Loteria online não funciona? Usuários reclamam de falhas no site da Caixa"* (techtudo.com.br) e *"Loterias Caixa fora do ar? Usuários reclamam de instabilidade para apostar na Mega"*.
- Durante a Mega da Virada, a fila para apostar no site chegou a **mais de três horas**, com usuários esperando entre 14h e 17h19 para conseguir acesso (dado agregado da busca, referenciando reportagens/reclamações).
- Mensagem de erro recorrente citada: "OPS, TIVEMOS UM PROBLEMA, ENTRE NOVAMENTE MAIS TARDE".
- Reclamações recorrentes de app travando "todos os dias entre 18h e 19h" por excesso de acesso simultâneo (padrão: horário de fechamento das apostas do dia).
- App trava na tela de "auto-avaliação obrigatória", impedindo o usuário de sequer abrir o app após uma atualização (Reclame Aqui, título "auto avaliação trava o aplicativo loterias caixa").
- Falhas recorrentes desde dezembro de 2024: app fecha sozinho e "não completa as ações solicitadas pelo usuário, impossibilitando conferir as apostas" (Reclame Aqui, snippet de busca).

**Implicação para o produto:** a instabilidade do canal oficial é fora do controle do Jogos Bem Feitos (é a própria Caixa), mas reforça o valor de qualquer camada que reduza o tempo de exposição do usuário ao site da Caixa (preenchimento rápido/automatizado) e que preserve os jogos gerados/organizados fora do sistema instável da Caixa (evitando perda de dados quando o carrinho "some").

### 1.3 Apostas e "carrinhos" que somem — perda de confiança no registro
Categoria de dor distinta e muito citada: usuários relatam perder o registro de apostas já feitas.

- Múltiplos títulos de Reclame Aqui: "Aposta na Lotofácil sumiu do aplicativo após o sorteio", "Opção 'minhas apostas' sumiu do app Loterias Caixa impossibilitando conferir jogos", "Carrinhos favoritos de apostas sumiram no site da Caixa", "Apostas da Lotofácil da Independência Sumiram do App Loterias Caixa", "Minhas apostas sumiram do site da Loterias Caixa".
- Achado importante (via busca, citando os termos da Caixa): **apostas que ficam apenas no carrinho não são consideradas finalizadas e não concorrem ao sorteio** — ou seja, parte da "perda" relatada por usuários é confusão de UX real da Caixa (aposta no carrinho ≠ aposta paga/confirmada), não necessariamente um bug. Isso é uma dor de **compreensão do fluxo de aposta**, não só técnica.
- Filtro padrão do histórico mostra só os últimos 7 dias, e o histórico completo só fica disponível por 6 meses — usuários reclamam de "sumiço" quando na verdade é um filtro/prazo (evidência de fricção de usabilidade que gera desconfiança).

**Implicação:** há espaço de valor real em manter um registro externo e confiável de "o que eu apostei, quando, e se paguei", robusto à instabilidade e às limitações de UX do site da Caixa — isso é essencialmente o "organizar jogos/apostas em grupos" do Jogos Bem Feitos, mas a evidência mostra que o problema vai além de "organização por preferência": é **credibilidade do registro** (o usuário não confia que o que fez ficou salvo).

### 1.4 Conferência manual de jogos
- Snippet de busca resume bem a dor: *"Conferir manualmente os jogos da Lotofácil demora e consome tempo. Muitas pessoas precisam conferir com caneta e bloquinho e correm o risco de esquecer de conferir seus volantes e perder prêmios."*
- Existe todo um mercado de apps dedicados só a isso: "Lotofácil - Verificar jogos" (Google Play), "Suas Apostas" (App Store, controla e confere Mega-Sena/Quina/Lotofácil com notificação minutos após o sorteio oficial), ConfiraLoterias, MazuSoft, Loterias Brasil.
- O risco citado — **esquecer de conferir e perder prazo de resgate de prêmio** — é uma dor de alta intensidade (perda financeira real, ainda que rara) combinada com frequência alta (toda aposta precisa ser conferida).

### 1.5 Organização de bolões/grupos e confiança na divisão do prêmio
Esta foi a categoria mais rica e com implicações diretas para o "organizar jogos/apostas em grupos" do produto — é claramente uma dor validada e ainda mal resolvida no mercado.

- Concorrente direto identificado: **BolãoBR** (bolaobr.com.br) — "Organize Bolões de Loteria Online sem Planilha". Copy do produto: permite *"criar grupos, compartilhar convites por link e acompanhar cotas, prazos e confirmações — tudo em um só lugar, sem cobrança manual nem planilha"*; lê automaticamente comprovantes de PIX e confere resultado oficial; tem bot no Telegram (@BolaoBRbot). Isso é evidência de mercado validando a dor "organizar bolão sem planilha" com disposição de construir um produto inteiro em torno disso.
- Outro concorrente: **LotoMaisFácil** (lotomaisfacil.com.br) — organiza bolões em grupos de WhatsApp "com transparência desde seu início" — o próprio posicionamento de marketing ("transparência") indica que a falta de transparência é a dor percebida no mercado informal.
- Fonte jornalística (Estado de Minas, fev/2026): *"Bolão da Lotofácil: como organizar um com amigos e não ter problemas"* — título já assume que "ter problemas" é a expectativa padrão.
- Achado central de risco (via busca, citando Folha Vitória / Serasa): em bolão informal, **só uma pessoa fica com o bilhete físico/registro**, a Caixa paga a quem apresenta o comprovante, e a divisão entre os demais depende inteiramente do organizador e de acordos informais. Uma mensagem de WhatsApp combinando cotas **não tem o mesmo valor legal/prático que o recibo individual emitido pela Caixa**.
- Recomendação oficial citada (Serasa/Folha Vitória): usar o **Bolão Caixa oficial**, que gera recibo de cota individual resgatável separadamente — sinal de que a solução "correta" já existe institucionalmente, mas o mercado claramente prefere/usa bolões informais via WhatsApp mesmo assim (por isso produtos como BolãoBR existem para preencher essa lacuna de confiança sem forçar todo mundo a usar o canal oficial).
- Contexto de golpe adjacente (não é o produto, mas contamina a percepção de risco do nicho): golpe do "bilhete premiado" onde criminosos fingem ter ganho e pedem dinheiro adiantado para "liberar o prêmio" (Estado de Minas).

**Implicação forte:** "organizar jogos em grupos" não é só uma feature de conveniência — ela resolve um problema de **confiança e comprovação** que hoje é preenchido de forma frágil (WhatsApp + planilha + palavra do organizador). Isso é uma dor de alta intensidade emocional (dinheiro + amizade em jogo) mesmo sendo de frequência mais baixa (só importa quando o grupo de fato ganha, mas a ansiedade existe o tempo todo).

### 1.6 Custo/orçamento das apostas com muitos números
- Dado concreto (Intersena, InfoFinanceira): jogar com 18 números na Lotofácil custa R$ 2.040; com 20 números, R$ 155.040 (aposta cheia individual) — números que tornam a estratégia de "fechamento" praticamente inacessível sem diluir em bolão.
- Recomendação recorrente encontrada: gastos com loteria não deveriam ultrapassar um percentual pequeno da renda; definir orçamento fixo mensal; usar bolão para "cobrir mais dezenas" dividindo custo (ex.: 20 números por ~R$ 1.938/pessoa em bolão de 20 cotas, citado por fonte agregada).
- Isso conecta diretamente "gerar jogos com IA/fechamento matemático" à necessidade de **dividir custo via bolão** — ou seja, geração e organização em grupo são funcionalidades que se reforçam mutuamente na jornada real do apostador que quer jogar "mais números com responsabilidade financeira".

### 1.7 Golpes, propaganda enganosa e produtos que prometem "IA" para prever loteria
Categoria de dor negativa (risco de o mercado desconfiar do próprio Jogos Bem Feitos por associação) — extremamente relevante para a estratégia de posicionamento e comunicação de "IA" do produto.

- **Loto Sniper / Loto Lógica**: mais de 300 relatos de golpe no Reclame Aqui (via snippet agregado de busca). Título de reclamação real: *"Não compre esse programa - TUDO MENTIRA E POSSO PROVAR"* (reclameaqui.com.br/loto-sniper). Outro título: *"Propaganda enganosa. Não cumpre com o que promete!"*.
- Alegação de marketing do produto golpista (capturada via busca): promete **"até 80% de acerto na Lotofácil"** usando "inteligência artificial" — promessa estatisticamente impossível e que a Caixa e checadores desmentem publicamente.
- Reclamações de usuários (paráfrase de busca): pagaram (ex.: R$ 197 citado para "Loto Lógica") e **não receberam link/acesso**, ou perderam acesso após a assinatura, sem ganhar dinheiro algum.
- Fact-check da Agência Lupa (25/set/2025): *"É golpe aplicativo que promete acertar números para ganhar na Loteria"* — a Caixa confirma publicamente que **não há brechas ou falhas nos sistemas de loteria que permitam prever ou influenciar os números sorteados**, e que os sorteios são conduzidos com total transparência e segurança física (não algorítmica).
- Vídeo denunciando especificamente: "Golpe do APP Loto Lógica - Fraude Comprovada" (YouTube).
- Existe também reclamação contra a própria Caixa alegando "App loteria da caixa é enganação" no Reclame Aqui — sinal de que a desconfiança do usuário médio de loteria é ampla, não se limita a apps de terceiros.

**Implicação crítica:** este é o ponto mais sensível para o Jogos Bem Feitos. O mercado já está saturado de produtos que usam a palavra "IA" para vender uma promessa impossível (prever sorteio), e há centenas de reclamações documentadas de fraude associadas a exatamente esse discurso. Qualquer comunicação do produto que sugira, mesmo implicitamente, "IA que aumenta suas chances de ganhar" corre risco de ser lida com o mesmo ceticismo — ou pior, atrair o público errado (quem busca "fórmula secreta") e depois gerar frustração/reclamação quando o produto (corretamente) não entrega previsão alguma.

---

## 2. Percepções sobre "IA" no contexto de loteria

**Fato vs. crença de mercado — separação explícita:**

- **Fato (consenso técnico/checado por fact-checkers e pela própria Caixa):** sorteios de loteria são eventos físicos aleatórios e estatisticamente independentes; não existe padrão oculto previsível por algoritmo, IA ou análise histórica. Fonte: Agência Lupa (agencialupa.org, 25/set/2025), citando a Caixa Federal diretamente: *"não há brechas ou falhas nos sistemas de loteria que permitam prever ou influenciar os números sorteados"*.
- **Crença de mercado (não é fato, é o que uma parte dos usuários acredita ou quer acreditar):** que "IA" pode "aumentar as chances de ganhar" ou até prever números. Essa crença é ativamente alimentada por:
  - Casos virais de "estudantes que usaram IA e ganharam" (caso real de estudantes italianos que ganharam €50 mil na loteria da Itália), amplamente noticiado em português (ndmais.com.br, marketeer.sapo.pt, vídeo do Tony Ventura no YouTube). **Importante**: mesmo as fontes que cobrem esse caso fazem a ressalva de que matemáticos afirmam que "o algoritmo não funcionaria a longo prazo" e que isso não prova capacidade preditiva — foi coberto midiaticamente de forma sensacionalista, mas o próprio conteúdo desmente a tese central quando lido com atenção.
  - Produtos concorrentes que exploram ativamente essa crença: **LotoAI** (lotoai.com.br — "Gerador de Jogos com IA... com estatísticas avançadas, análise de padrões e dashboard analítico"), **Sortiq** (sortiq.com.br — usa "Machine Learning, Lei de Benford e análise de momentum para otimizar jogos da Mega-Sena" — uso de "Lei de Benford" aplicado a sorteio aleatório é matematicamente questionável, já que a Lei de Benford se aplica a dados que seguem certas distribuições de ocorrência natural, não a sorteios uniformemente aleatórios), e **IA da Loteria** (iadaloteria.com.br).
  - No extremo golpista, "Loto Sniper"/"Loto Lógica" promete explicitamente 80% de acerto via "IA" — e gerou centenas de reclamações de fraude.

**Leitura crítica para o Jogos Bem Feitos:** o mercado já tem pelo menos três concorrentes (LotoAI, Sortiq, IA da Loteria) usando "IA" como gancho de marketing para geração/análise de jogos, num espectro que vai do razoavelmente honesto (geração assistida, organização, estatística descritiva) até o francamente fraudulento (promessa de % de acerto). O risco reputacional de usar "IA" no posicionamento é real e comprovado por mais de 300 reclamações documentadas contra um único concorrente. Isso não significa evitar a palavra IA, mas sim que a comunicação precisa deixar claríssimo — de forma até mais explícita que a concorrência "séria" — que o valor da IA está em geração/organização/copiloto conversacional (Trevin) e não em previsão ou aumento de probabilidade estatística real de acerto. Não encontrei evidência de que usuários comuns (fora do público que já caiu em golpe) tratem "gerar jogos com IA" como sinônimo de "prever números" — a maior parte da linguagem de mercado saudável (fechamentos, desdobramentos) é sobre **cobertura matemática de combinações**, não previsão.

---

## 3. Percepções sobre automação/preenchimento manual de apostas

- Preenchimento manual de muitas apostas (comum em fechamentos com muitas dezenas ou bolões grandes) é percebido como trabalho tedioso e sujeito a erro — evidenciado pela existência de um pequeno ecossistema de extensões gratuitas/independentes dedicado só a isso (seção 1.1).
- A confiança é a principal barreira de adoção de qualquer ferramenta que "mexe" no site da Caixa: as duas extensões mais citadas fazem questão de declarar publicamente que não coletam login, senha ou dados pessoais, e uma delas ("Automação Loterias Caixa") reforça explicitamente que "a conferência e a finalização da aposta permanecem sob responsabilidade do usuário" — ou seja, o próprio concorrente evita se posicionar como responsável pela transação financeira final, mantendo o usuário no controle do clique final de pagamento. Isso é um padrão de mercado relevante: **automatizar o preenchimento, mas não a confirmação/pagamento**, para reduzir a percepção de risco.
- A instabilidade do site da Caixa (seção 1.2) tende a amplificar a necessidade de automação: quanto mais lento e instável o site oficial, maior o valor percebido de preencher rápido antes de travar ou expirar a sessão, e mais crítico é ter os jogos já prontos/organizados fora do site antes de tentar submeter.
- Não encontrei reclamações específicas contra as próprias extensões automatizadoras alegando perda de dinheiro ou erro de preenchimento — o volume de reviews é baixo (12 avaliações na maior extensão encontrada) demais para tirar conclusões fortes sobre confiabilidade técnica; é uma lacuna de evidência, não uma confirmação de que funcionam bem.

---

## 4. Jobs To Be Done — classificados

Legenda de evidência: **[E]** = baseado em evidência direta encontrada; **[I]** = inferência razoável a partir do conjunto de evidências (marcado como tal).

### JTBD 1 — Preencher apostas rapidamente sem erro
**"Quando eu já decidi quais jogos vou apostar (especialmente vários jogos ou um fechamento grande), quero preenchê-los no site da Caixa de forma rápida e automática, para não perder tempo digitando manualmente e não errar números por cansaço/pressa."**
- Frequência: **Alta** [E] — toda aposta múltipla passa por isso; existe todo um mercado de extensões dedicadas.
- Intensidade da dor: **Média** [E] — irritante e demorado, mas não impede a aposta (existe workaround manual).
- Disposição a pagar: **Média** [I] — extensões concorrentes são majoritariamente gratuitas/independentes, o que sugere baixa disposição a pagar só por isso isoladamente, mas alta disposição quando empacotado com geração+organização.
- Qualidade das soluções atuais: **Mediana** [E] — extensões existem, mas com poucos usuários (770 instalações a mais popular encontrada), nota 3.7/5, baixo volume de reviews, sem grande empresa por trás.
- Oportunidade para Jogos Bem Feitos: **Alta** — já é uma feature do produto (extensão Chrome); a concorrência é fragmentada, pouco profissional e feita por devs individuais sem suporte robusto, deixando espaço para uma solução integrada com geração+organização+preenchimento em um fluxo único.

### JTBD 2 — Não perder o registro do que foi apostado
**"Quando eu faço várias apostas ao longo do tempo, quero ter um registro confiável e centralizado de tudo que apostei (mesmo se o site da Caixa 'sumir' com o histórico ou aplicar filtros que escondem apostas antigas), para ter certeza de que sei exatamente o que joguei e quando."**
- Frequência: **Alta** [E] — toda aposta recorrente gera esse risco; múltiplas reclamações de "apostas sumiram".
- Intensidade da dor: **Alta** [E] — envolve medo de perder prêmio, e há relatos de usuários achando que perderam apostas (mesmo que parte seja mal-entendido de UX/filtro da Caixa).
- Disposição a pagar: **Média-Alta** [I] — está diretamente ligado a dinheiro e ansiedade financeira, o que costuma elevar disposição a pagar por tranquilidade.
- Qualidade das soluções atuais: **Ruim** [E] — a própria Caixa é a fonte do problema (filtros de 7 dias, "sumiço" de carrinhos favoritos, limite de 6 meses de histórico); não há concorrente claro resolvendo isso de forma independente do site oficial.
- Oportunidade para Jogos Bem Feitos: **Alta** — organizar jogos em um sistema próprio, fora da dependência do site instável da Caixa, ataca diretamente essa dor e é diferenciação real frente a "gerador de números" genérico.

### JTBD 3 — Conferir resultados sem esquecer nem perder prazo
**"Quando o sorteio sai, quero saber automaticamente se acertei (e quanto), para não precisar conferir manualmente com caneta/bloquinho e não correr risco de esquecer e perder o prazo de resgate do prêmio."**
- Frequência: **Alta** [E] — toda aposta precisa ser conferida, múltiplas vezes por semana para quem joga várias loterias.
- Intensidade da dor: **Alta** [E] — risco de perda financeira real (prazo de resgate) é citado explicitamente como consequência do esquecimento.
- Disposição a pagar: **Média** [I] — já existem várias soluções gratuitas robustas (apps dedicados, sites), o que tende a reduzir disposição a pagar só por essa feature isolada.
- Qualidade das soluções atuais: **Boa** [E] — mercado maduro de apps de conferência (Suas Apostas, ConfiraLoterias, MazuSoft, Loterias Brasil), com notificação minutos após o sorteio.
- Oportunidade para Jogos Bem Feitos: **Média** — feature necessária para completude do produto (fechar o ciclo gerar→apostar→conferir), mas não é diferenciação competitiva por si só, já que o mercado já resolve isso razoavelmente bem de graça.

### JTBD 4 — Organizar um bolão/grupo com transparência e sem depender de planilha
**"Quando eu organizo (ou participo de) uma aposta em grupo com amigos/família/colegas, quero ter clareza de quem pagou, quantas cotas cada um tem e como o prêmio será dividido, para evitar brigas, desconfiança ou perda de dinheiro por falta de comprovação."**
- Frequência: **Média** [E] — bolões são comuns mas não diários; picos em datas especiais (Mega da Virada, prêmios acumulados).
- Intensidade da dor: **Alta** [E] — envolve dinheiro + relações pessoais; artigos e produtos inteiros (BolãoBR, LotoMaisFácil) existem só para isso; risco documentado de disputa quando só uma pessoa fica com o comprovante oficial.
- Disposição a pagar: **Alta** [I] — BolãoBR é um produto pago construído inteiramente em torno dessa dor, validando disposição a pagar por resolver especificamente "confiança + praticidade" em bolões.
- Qualidade das soluções atuais: **Mediana** [E] — BolãoBR e LotoMaisFácil existem e têm proposta de valor clara (leitura automática de PIX, bot Telegram), mas são players pequenos e o padrão de mercado ainda é WhatsApp + planilha informal, que não tem validade legal equivalente ao recibo oficial da Caixa.
- Oportunidade para Jogos Bem Feitos: **Alta** — "organizar jogos/apostas em grupos" já é pilar do produto; a evidência mostra que essa é uma das dores mais fortes e menos resolvidas do mercado, com concorrência direta mas ainda pequena/fragmentada.

### JTBD 5 — Cobrir mais números sem estourar o orçamento sozinho
**"Quando eu quero aumentar minhas chances jogando com mais dezenas (fechamento), quero saber quanto isso custa e como dividir esse custo com outras pessoas, para poder jogar 'grande' sem comprometer meu orçamento individual."**
- Frequência: **Média** [E] — relevante sempre que o usuário considera fechamentos com 16+ dezenas; custo sobe exponencialmente (18 números = R$2.040; 20 números = R$155.040).
- Intensidade da dor: **Média-Alta** [I] — é uma barreira de entrada real para estratégias mais "sérias" de aposta; conecta diretamente geração de jogos com necessidade de bolão.
- Disposição a pagar: **Média** [I] — usuários que already gastam centenas/milhares em fechamento tendem a ter mais disposição a pagar por uma ferramenta que otimiza esse investimento.
- Qualidade das soluções atuais: **Mediana** [E] — calculadoras de custo existem (Intersena, InfoFinanceira) mas são estáticas/informativas, não integradas a um fluxo de geração+divisão de cotas.
- Oportunidade para Jogos Bem Feitos: **Alta** — combinar geração de jogos com fechamento + simulação de custo + divisão automática de cotas em grupo é uma integração que nenhum concorrente parece oferecer de forma unificada (BolãoBR não gera jogos com IA; LotoAI/Sortiq não organizam bolão).

### JTBD 6 — Confiar que o produto que usa "IA" não é um golpe disfarçado
**"Quando eu considero pagar por um app ou serviço que promete gerar jogos com 'IA', quero ter sinais claros de que não é uma fraude que vai me cobrar e sumir, para não repetir a experiência de quem perdeu dinheiro com apps como Loto Sniper/Loto Lógica."**
- Frequência: **Baixa-Média** [I] — é um momento pontual (decisão de compra), mas relevante para todo novo usuário em potencial.
- Intensidade da dor: **Alta** [E] — mais de 300 reclamações documentadas de fraude associada a "IA + loteria"; a categoria inteira carrega estigma.
- Disposição a pagar: N/A (é uma barreira à disposição a pagar, não um job pago em si).
- Qualidade das soluções atuais: **Ruim** [E] — o próprio mercado é a origem do problema (concorrentes fraudulentos convivem lado a lado com os legítimos, sem diferenciação clara para o usuário leigo).
- Oportunidade para Jogos Bem Feitos: **Alta** — não é uma feature de produto, mas um imperativo de posicionamento/comunicação: transparência ativa sobre o que a IA faz (organiza, gera, conversa) e não faz (não prevê, não garante prêmio) pode se tornar vantagem competitiva de confiança, especialmente com prova social real (Reclame Aqui próprio, depoimentos verificáveis, clareza de preço sem "trial que vira cobrança escondida" — ver JTBD 7).

### JTBD 7 — Não ser pego de surpresa por cobrança de assinatura
**"Quando eu assino um app de loteria (inclusive em período de teste gratuito), quero saber exatamente quando e quanto vou ser cobrado e conseguir cancelar facilmente, para não ter que registrar reclamação de cobrança indevida depois."**
- Frequência: **Média** [I] — relevante no momento de conversão/renovação de assinatura, recorrente mensalmente/anualmente.
- Intensidade da dor: **Alta** [E] — múltiplas reclamações no Reclame Aqui sobre "cobrança indevida de assinatura anual após promessa de avaliação gratuita" e dificuldade de cancelamento em apps do nicho (LotoApp citado com renovação automática problemática).
- Disposição a pagar: N/A (dor sobre o processo de pagamento, não um job pago à parte).
- Qualidade das soluções atuais: **Ruim** [E] — padrão de mercado (trial que converte em cobrança sem aviso claro) é fonte recorrente de reclamação em SaaS de loteria e fora dele.
- Oportunidade para Jogos Bem Feitos: **Média-Alta** — diferenciação simples via política de cobrança transparente, lembrete antes de cobrar, cancelamento sem fricção — baixo custo de implementação, alto potencial de reduzir churn por raiva/desconfiança.

### JTBD 8 — Gerar jogos com "método" sem precisar entender estatística
**"Quando eu não sei/não quero estudar estatística, fechamentos e desdobramentos matemáticos sozinho, quero que um assistente monte isso para mim de forma conversacional, para aplicar estratégias (equilíbrio par/ímpar, evitar padrões óbvios, fechamentos) sem precisar ser especialista."**
- Frequência: **Alta** [E] — a quantidade de conteúdo (guias, blogs, PDFs "método infalível") sobre "dicas para lotofácil" indica demanda alta e recorrente por orientação.
- Intensidade da dor: **Média** [I] — não é bloqueante (dá pra jogar números aleatórios), mas há desejo claro de "jogar melhor" e insegurança sobre como fazer isso corretamente.
- Disposição a pagar: **Média-Alta** [E] — existência de múltiplos produtos pagos (LotoAI, Sortiq, IA da Loteria, LotoCarva com "413 fechamentos profissionais" via assinatura) mostra mercado dado a pagar por esse tipo de orientação/ferramenta.
- Qualidade das soluções atuais: **Mediana** [E] — ferramentas de geração/fechamento existem, mas maioria é baseada em formulário estático (escolher parâmetros, gerar lista), não conversacional; um "copiloto" via linguagem natural (Trevin) é diferenciação real frente ao padrão de mercado.
- Oportunidade para Jogos Bem Feitos: **Alta** — Trevin, como assistente conversacional, ataca esse job de forma mais natural que os geradores estáticos concorrentes, desde que a comunicação evite prometer "aumento de chance real" (ver seção 2) e foque em "aplicar estratégias de cobertura/organização de forma acessível".

### JTBD 9 — Jogar dentro do orçamento sem se sentir "viciado"
**"Quando eu percebo que estou gastando mais do que planejava em apostas, quero ferramentas que me ajudem a definir e respeitar um limite, para manter o jogo como lazer controlado e não como um problema financeiro."**
- Frequência: **Baixa-Média** [I] — relevante para uma parcela dos apostadores mais frequentes/pesados, não a maioria ocasional.
- Intensidade da dor: **Alta** (quando presente) [E] — conteúdo específico sobre "vício em apostas" e recomendação de não ultrapassar determinado % da renda em lazer indica que é uma preocupação real documentada, mesmo que nicho.
- Disposição a pagar: **Baixa** [I] — é um job mais de "responsabilidade"/bem-estar do que de conveniência; historicamente esse tipo de feature (limites de gasto) é oferecido de graça por reguladores/plataformas de apostas esportivas, não vendido.
- Qualidade das soluções atuais: **Ruim/inexistente** [I] — não encontrei ferramenta específica de controle de orçamento integrada a apps de geração de jogos de loteria (diferente de apostas esportivas, que já tem "jogo responsável" mais maduro).
- Oportunidade para Jogos Bem Feitos: **Média** — não é core, mas pode ser um recurso de baixo custo (ex.: Trevin alertando sobre valor total do fechamento antes de confirmar) que constrói confiança e diferenciação ética, coerente com o JTBD 6 (combater percepção de "app de loteria oportunista").

### JTBD 10 — Decidir rapidamente entre "aposta simples" e "fechamento" sem se perder em opções
**"Quando eu não sei se vale a pena fazer um fechamento com mais dezenas ou apostar simples, quero uma simulação clara de custo x cobertura, para decidir com confiança quanto vou gastar e o que estou comprando com isso."**
- Frequência: **Média** [I] — decisão tomada a cada "aposta grande", não a cada aposta simples do dia a dia.
- Intensidade da dor: **Média** [E] — os artigos que explicam "quanto custa 18/20 números" e "como calcular" indicam que essa é uma dúvida recorrente e não trivial (números como R$155 mil para 20 dezenas surpreendem o usuário leigo).
- Disposição a pagar: **Média** [I] — ligado ao mesmo bolso do JTBD 5 (cobrir mais números / dividir custo).
- Qualidade das soluções atuais: **Mediana** [E] — calculadoras estáticas existem (Utilitários Online, Intersena) mas não integradas a um gerador+organizador de grupo real.
- Oportunidade para Jogos Bem Feitos: **Média-Alta** — combinar simulação de custo diretamente na geração de jogos e no fluxo de bolão (JTBD 4) fecha um funil que hoje está espalhado em ferramentas separadas.

### JTBD 11 — Confirmar que a extensão/ferramenta não vai mexer no meu dinheiro sem eu perceber
**"Quando eu instalo uma extensão que interage com o site oficial da Caixa (onde há dinheiro e login envolvidos), quero ter certeza de que ela não vê minha senha, não faz pagamento sozinha e me deixa no controle da confirmação final, para usar a automação sem medo de fraude ou erro."**
- Frequência: **Baixa** [I] — ocorre uma vez, no momento da instalação/primeira confiança, mas é um pré-requisito para todo o resto.
- Intensidade da dor: **Alta** [E] — todas as extensões concorrentes fazem questão de declarar explicitamente que não coletam login/senha e que a confirmação final fica com o usuário — um sinal forte (revealed behavior dos próprios concorrentes) de que essa é a objeção nº1 antes de instalar.
- Disposição a pagar: N/A (é uma barreira de adoção, não um job pago à parte).
- Qualidade das soluções atuais: **Mediana** [E] — concorrentes já adotam a postura correta (não pedir credenciais, manter usuário no controle do pagamento), mas a comunicação disso é informal (texto solto na descrição da loja), não um selo de confiança robusto.
- Oportunidade para Jogos Bem Feitos: **Média-Alta** — reforçar ativamente essa garantia (política clara, talvez auditável/open sobre o que a extensão faz) é baixo custo e resolve a principal barreira de conversão para a feature de preenchimento automático.

### JTBD 12 — Ter um canal estável para apostar quando o site oficial trava
**"Quando o site/app da Caixa está lento ou fora do ar (especialmente em horários de pico ou datas especiais como a Mega da Virada), quero ter meus jogos prontos e organizados para inserir assim que o sistema voltar, para não perder a janela de tempo até o fechamento das apostas."**
- Frequência: **Média** [E] — picos recorrentes de instabilidade (18h-19h diariamente, e picos extremos em datas especiais) documentados em múltiplas reclamações e reportagens (TechTudo).
- Intensidade da dor: **Alta** (nos picos) [E] — fila de até 3h+ registrada na Mega da Virada; risco real de não conseguir apostar a tempo.
- Disposição a pagar: **Baixa-Média** [I] — o problema é da Caixa, não algo que o produto resolve diretamente, mas pode mitigar (jogos pré-montados prontos para inserção rápida assim que o acesso volta).
- Qualidade das soluções atuais: **Ruim** [E] — nenhum concorrente parece endereçar isso especificamente; é uma falha estrutural do canal oficial.
- Oportunidade para Jogos Bem Feitos: **Média** — não é solucionável diretamente, mas o produto pode se posicionar como "prepare tudo com antecedência para não depender da velocidade do site no momento crítico", transformando uma dor de terceiros em razão de uso do produto.

---

## 5. Lista de Fontes

**Reclame Aqui (via snippets de busca — acesso direto bloqueado com HTTP 403 na maioria das tentativas):**
- reclameaqui.com.br/loto-sniper/nao-compre-esse-programa-tudo-mentira-e-posso-provar
- reclameaqui.com.br/loto-sniper/propaganda-enganosa
- reclameaqui.com.br/loto-sniper/propogana-enganosa
- reclameaqui.com.br/loto-sniper/loto-logica
- reclameaqui.com.br/empresa/loto-sniper/lista-reclamacoes
- reclameaqui.com.br/empresa/loto-logica/lista-reclamacoes
- reclameaqui.com.br/empresa/loteria-digital/lista-reclamacoes
- reclameaqui.com.br/empresa/loteriasoft/lista-reclamacoes
- reclameaqui.com.br/caixa-economica-federal/app-loteria-da-caixa-e-enganacao
- reclameaqui.com.br/caixa-economica-federal/problemas-de-acesso-ao-site-loterias-caixa-ja-tem-algumas-semanas
- reclameaqui.com.br/caixa-economica-federal/problemas-com-o-aplicativo-de-loterias-da-caixa-dificuldades-de-acesso-apostas-e-resgate-de-premios
- reclameaqui.com.br/caixa-economica-federal/app-loterias-caixa-travado
- reclameaqui.com.br/caixa-economica-federal/auto-avaliacao-trava-o-aplicativo-loterias-caixa
- reclameaqui.com.br/caixa-economica-federal/aplicativo-loterias-caixa-nao-funciona
- reclameaqui.com.br/caixa-economica-federal/app-loterias-esta-travando-sempre-no-fim-do-dia
- reclameaqui.com.br/caixa-economica-federal/aposta-na-lotofacil-sumiu-do-aplicativo-apos-o-sorteio
- reclameaqui.com.br/caixa-economica-federal/opcao-minhas-apostas-sumiu-do-app-loterias-caixa-impossibilitando-conferir-jogos
- reclameaqui.com.br/caixa-economica-federal/carrinhos-favoritos-de-apostas-sumiram-no-site-da-caixa
- reclameaqui.com.br/google-brasil/google-play-cobranca-indevida-e-recusa-de-reembolso-para-assinatura-de-app-nao-atendente-as-necessidades

**Fact-checking / jornalismo:**
- [É golpe aplicativo que promete acertar números para ganhar na Loteria – Agência Lupa](https://www.agencialupa.org/jornalismo/2025/09/25/e-golpe-aplicativo-que-promete-acertar-numeros-para-ganhar-na-loteria/)
- [Loteria online não funciona? Usuários reclamam de falhas no site da Caixa – TechTudo](https://www.techtudo.com.br/noticias/2024/12/loteria-online-nao-funciona-usuarios-reclamam-de-falhas-no-site-da-caixa-edsoftwares.ghtml)
- [Loterias Caixa fora do ar? Usuários reclamam de instabilidade para apostar na Mega – TechTudo](https://www.techtudo.com.br/noticias/2024/12/loterias-caixa-fora-do-ar-usuarios-reclamam-de-instabilidade-para-apostar-na-mega-edsoftwares.ghtml)
- [Bolão da Lotofácil: como organizar um com amigos e não ter problemas – Estado de Minas](https://www.em.com.br/trends/2026/02/7364383-bolao-da-lotofacil-como-organizar-um-com-amigos-e-nao-ter-problemas.html)
- [Bolão entre amigos deu prêmio? Guia para não ter problemas na hora – Estado de Minas](https://www.em.com.br/trends/2026/01/7342352-bolao-entre-amigos-deu-premio-guia-para-nao-ter-problemas-na-hora.html)
- [Bolão da loteria: 7 erros que podem custar o prêmio – Folha Vitória](https://www.folhavitoria.com.br/loterias/vai-entrar-em-um-bolao-7-erros-podem-fazer-voce-perder-um-premio-milionario/)
- [Saiba identificar o golpe do bilhete premiado – Estado de Minas](https://www.em.com.br/emfoco/2025/05/26/saiba-identificar-o-golpe-do-bilhete-premiado-e-como-evitar-cair-nessa-fraude/)
- [Como participar de um bolão: dicas e regras essenciais – Serasa](https://www.serasa.com.br/blog/bolao/)
- [Três estudantes usam a inteligência artificial para prever a loteria e ganham R$ 265 mil – ND Mais](https://ndmais.com.br/loterias/tres-estudantes-usam-a-inteligencia-artificial-para-prever-a-loteria-e-ganham-r-265-mil/)
- [Será mesmo possível ganhar a lotaria através da inteligência artificial? – Marketeer](https://marketeer.sapo.pt/sera-mesmo-possivel-ganhar-a-lotaria-atraves-da-inteligencia-artificial-tres-estudantes-de-matematica-desafiaram-a-sorte/)
- [Lotofácil: 5 dicas e estratégias – Estado de Minas](https://www.em.com.br/trends/2026/02/7360748-lotofacil-5-dicas-e-estrategias-para-aumentar-suas-chances-de-ganhar.html)
- [Quanto Custa Jogar 18 Números na Lotofácil – Intersena](https://www.intersena.com.br/lotofacil/quanto-custa-jogar-18-numeros-lotofacil)
- [Quanto custa 18 números na Lotofácil? – InfoFinanceira](https://infofinanceira.com.br/quanto-custa-18-numeros-lotofacil/)
- [Lotofácil: jogo de sorte ou risco financeiro? – Quero Quitar](https://www.queroquitar.com.br/blog/organizacao/lotofacil-jogo-de-sorte-ou-risco-financeiro/)

**Produtos/concorrentes (páginas próprias, via busca e fetch parcial):**
- [Apostas automáticas Loterias Caixa – Chrome Web Store](https://chromewebstore.google.com/detail/apostas-autom%C3%A1ticas-loter/lleccpmgmkoajogkgmnpbgoodgebpnlb) (fetch direto: 770 instalações, 3.7/5, 12 avaliações)
- [Automação Loterias Caixa – Chrome Web Store](https://chromewebstore.google.com/detail/automa%C3%A7%C3%A3o-loterias-caixa/ndlbkaamjcndgcjhhcbneeignadioohf)
- [ChromeLoteca – GitHub](https://github.com/LukeC8/chromeloteca)
- [INJOLOCA – GitHub](https://github.com/guynovaes/INJOLOCA)
- [JLP Apostas – Joga Loterias Profissional](https://www.jogaloterias.com.br/chrome-extensao-jlp-apostas)
- [BolãoBR – Organize Bolões de Loteria Online sem Planilha](https://bolaobr.com.br/)
- [LotoMaisFácil](https://lotomaisfacil.com.br/)
- [LotoAI – Gerador de Jogos com IA](https://www.lotoai.com.br/produto)
- [Sortiq – Análise de Loterias com IA e Machine Learning](https://sortiq.com.br/)
- [IA da Loteria](https://www.iadaloteria.com.br/)
- [LotoCarva – Gerador de Jogos](https://lotocarva.com/gerador-de-jogos/mega-sena)

**Google Play (dados agregados via busca, acesso a reviews individuais limitado):**
- play.google.com/store/apps/details?id=br.gov.caixa.loterias.apostas
- play.google.com/store/apps/details?id=com.hamanoapps.geradordeapostas
- play.google.com/store/apps/details?id=com.matrix.lotofacilfecha
- play.google.com/store/apps/details?id=br.com.fechamentos.lotofacil
- play.google.com/store/apps/details?id=br.com.estudiowebapps.lotofacil (Lotofácil - Verificar jogos)

---

## Observação final para a análise estratégica

O achado mais acionável desta pesquisa é que a maior dor validada e menos bem resolvida no mercado atual **não é a geração de jogos em si** (esse mercado já está saturado, inclusive de forma questionável com promessas de "IA que aumenta chance de ganhar"), mas sim **a organização de bolões com confiança/comprovação** e **a continuidade do registro de apostas fora da instabilidade do site oficial da Caixa**. Esses dois pontos combinados são exatamente onde "gerar jogos com IA" + "organizar em grupos" + "preencher automaticamente" se reforçam como um fluxo integrado — e é justamente essa integração ponta a ponta que nenhum concorrente identificado (BolãoBR, LotoAI, Sortiq, extensões de preenchimento) parece oferecer sozinho hoje.
