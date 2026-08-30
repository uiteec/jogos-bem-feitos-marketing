# REEL: "EU SOU O TREVIN" (STORYBOARD COMPLETO)

> **Este arquivo é a referência/storyboard completo, para leitura.** Para gerar no Veo, use os 7 prompts prontos e independentes na pasta [prompts/](prompts/) (um arquivo por clipe: `01-gancho`, `02-introducao`, `03a-gerador`, `03b-extensao-caixa`, `03c-meus-jogos`, `03d-bolao`, `04-cta`), já que cada um contém todas as regras necessárias (identidade do Trevin, telas do produto, pronúncia, voz etc.) porque o Veo não guarda contexto entre gerações.
>
> **Mudança importante:** os prompts em `prompts/` não anexam mais foto do Trevin. Em vez disso, incluem o bloco **CHARACTER LOCK: TREVIN** (descrição textual completa do personagem, definida em `prompts-base/prompt-trevin-atavatar.md`) diretamente no texto do prompt, em toda geração onde ele aparece. As instruções de "imagem como frame inicial" deste arquivo abaixo (seção 0.2 e regra 2) valem só para as screenshots reais do produto, não mais para o personagem.

Crie um vídeo publicitário vertical, moderno e profissional para Instagram Reels e TikTok apresentando **Trevin**, o assistente inteligente da plataforma **Jogos Bem Feitos**.

O vídeo funciona como o **"episódio piloto" de uma série de conteúdos**: apresenta o Trevin com calma, explica pra quem é o produto e o que ele faz, e cria expectativa para os próximos vídeos. Ritmo pausado e didático: não é mais um trailer picotado, é uma apresentação que alguém que nunca ouviu falar do Trevin consegue acompanhar e entender.

---

# 0. COMO GERAR ISSO NO VEO 3 / FLOW (LEIA ANTES DE GERAR)

**Texto sozinho não garante consistência de personagem nem de tela.** O modelo não "lembra" de uma imagem só porque ela foi descrita ou anexada uma vez lá no início: a cada geração ele desenha o personagem e as interfaces do zero a partir da descrição em texto, por isso o rosto muda e as telas são inventadas mesmo com as regras 2, 2.1 e 9 escritas no prompt.

## 0.1 Não gerar o vídeo inteiro de uma vez

Gerar **parte por parte** (ver instruções em cada parte abaixo sobre qual imagem anexar), depois editar os pedaços juntos em CapCut/Premiere para montar o corte final, sem esperar que o Veo entregue o vídeo inteiro pronto num prompt só.

## 0.2 "Anexar imagem de referência" ≠ "usar como primeiro frame": use a segunda opção

Existem dois jeitos de dar uma imagem pro Veo/Flow, e eles têm força bem diferente:

* **Imagem de referência/estilo ("Ingredients to Video"):** o modelo só se *inspira* nela. É fraco: ele ainda "redesenha" o personagem/tela com liberdade, e é exatamente aí que ele troca o rosto do Trevin ou inventa uma interface de video game.
* **Imagem como frame inicial ("Image to Video" / "Frames to Video"):** o modelo começa literalmente daqueles pixels e anima a partir dali. É muito mais forte para manter identidade, porque ele não tem liberdade de redesenhar o quadro de abertura, só de animar o que já está na imagem.

**Sempre que o Flow oferecer a opção, usar a imagem como frame inicial (image-to-video), não só como referência de estilo.** Quando usar frame inicial, escrever o texto do prompt só com a ação/câmera (ex: "aproximação sutil de câmera, Trevin pisca") e **não redescrever a aparência do personagem ou da tela**, pois a imagem já carrega isso; texto competindo com a imagem é o que causa a deriva.

Se a cena exigir um enquadramento que a imagem de referência ainda não tem (ex: Trevin integrado a uma interface específica), primeiro editar/compor essa imagem exata em uma ferramenta de imagem (Nano Banana, Photoshop, o próprio editor de imagem do Flow) partindo da referência original, e só then usar essa nova imagem estática como frame inicial do vídeo. Nunca pedir pro modelo de vídeo compor a cena inteira a partir do zero via texto.

## 0.3 Cada geração do Veo 3 sai com ~8 segundos, sem exceção

Não dá para pedir um trecho de 3s diretamente: cada geração vai sair com a duração fixa do modelo (por volta de 8s). O jeito de usar isso:

* Gerar cada trecho como um clipe cheio de ~8s (com a imagem certa como frame inicial e o movimento de câmera descrito).
* No editor, **cortar apenas o pedaço necessário** daquele clipe (ex: da Parte 1, usar só os 3 primeiros segundos; de cada tela da Parte 3, usar os ~2–3s em que ela aparece estável antes de cortar pra próxima).
* Isso significa gerar bem mais clipes do que partes no roteiro: cada trecho com imagem de referência diferente (Parte 1, Parte 2, cada uma das 4 telas da Parte 3, Parte 4) é uma geração de ~8s própria, depois cortada no tamanho certo.
* **Importante nesta versão:** diferente da v1, aqui cada tela precisa ficar tempo suficiente pra ser lida e entendida (mínimo 2–3s), nunca um flash de 0,5–1s. Prefira cortar o clipe de 8s pegando o trecho mais estável (sem muito movimento de câmera) em vez de um recorte curtíssimo.

## 0.4 "Jogos" = apostas de loteria, nunca video game

Toda vez que o prompt disser "jogos", "gerador de jogos" ou similar, isso significa **combinações numéricas de apostas de loteria** (grades de números, como nas telas reais anexadas), nunca jogos eletrônicos, consoles, controles, pixel art ou telas de arcade. Se o Veo gerar qualquer coisa parecida com video game, é sinal de que ele não recebeu a screenshot real como frame inicial (ver 0.2); nesse caso, regenerar anexando a imagem certa.

---

# 1. FORMATO DO VÍDEO

* Formato vertical **9:16**
* Instagram Reels / TikTok
* Duração aproximada: **30 segundos** (mais longo que a v1 anterior, de propósito, para dar tempo de entender)
* Ritmo **pausado e didático**, não acelerado
* Edição moderna
* Estética de campanha profissional de startup/SaaS
* Motion design clean
* Interface do produto como protagonista
* Poucos elementos simultâneos
* Nenhum texto ou legenda na tela
* Visual tecnológico sem exageros

O resultado deve parecer uma peça produzida profissionalmente para lançamento de um produto digital brasileiro, com um narrador que explica com calma, e não um teaser picotado.

NÃO deve parecer um vídeo genérico produzido por inteligência artificial.

---

# 2. REGRA CRÍTICA: IDENTIDADE DO TREVIN

A imagem anexada do personagem é uma **REFERÊNCIA VISUAL OBRIGATÓRIA DE IDENTIDADE**.

## O PERSONAGEM DA IMAGEM ANEXADA É O TREVIN.

Não utilize a imagem apenas como inspiração.

Não crie uma versão semelhante.

Não crie outro mascote.

Não redesenhe o personagem.

Não reinterprete seu design.

**USE E PRESERVE O PERSONAGEM FORNECIDO.**

**A cor do Trevin não pode ser alterada em nenhuma cena.** Manter exatamente as mesmas cores da imagem de referência do início ao fim do vídeo, mesmo com mudanças de iluminação, cena ou fundo.

A aparência do Trevin durante todo o vídeo deve permanecer visualmente consistente com a imagem anexada.

Preservar fielmente:

* formato da cabeça;
* formato do rosto;
* proporções;
* olhos;
* expressão;
* trevo ao redor da cabeça;
* formato do trevo;
* cores;
* detalhes visuais;
* estilo de ilustração;
* acabamento;
* personalidade visual.

## NÃO FAZER:

* não criar outro personagem baseado nele;
* não alterar seu rosto;
* não alterar seus olhos;
* não alterar o formato do trevo;
* não trocar suas cores;
* não adicionar cabelo;
* não adicionar acessórios;
* não adicionar corpo;
* não adicionar braços;
* não adicionar pernas;
* não transformar em humano;
* não transformar em robô;
* não transformar em personagem 3D;
* não transformar em personagem estilo Pixar;
* não deixar mais fofo;
* não infantilizar;
* não criar uma "versão moderna" dele.

Se for necessário animar Trevin, realizar apenas **microanimações compatíveis com a imagem original**, preservando sua identidade.

Exemplos permitidos:

* piscar suavemente;
* pequena movimentação dos olhos;
* mudança mínima de expressão;
* pequeno movimento natural da cabeça/personagem;
* aproximação da câmera.

A animação deve partir da identidade visual existente.

**A imagem fornecida representa o personagem final, e não um conceito a ser reinterpretado.**

---

# 2.1 REGRA CRÍTICA: TELAS DO SISTEMA

**Não gerar nenhuma tela, interface ou elemento de produto que não tenha sido fornecido como imagem de referência.**

Somente as telas anexadas como imagem podem aparecer no vídeo.

Não inventar:

* telas do gerador;
* telas de "Meus Jogos";
* telas de jogadores/bolão;
* painel da extensão;
* qualquer outra tela do Jogos Bem Feitos que não tenha sido explicitamente enviada como referência visual.

Se uma parte descrever uma funcionalidade (gerador, extensão, Meus Jogos, bolão etc.) e a tela correspondente **não** tiver sido fornecida como imagem, não criar uma versão fictícia dessa interface.

Nesse caso, resolver a cena sem mostrar tela de produto: usar Trevin, elementos gráficos simples ou composição abstrata, nunca uma interface inventada.

**Toda tela do sistema que aparecer no vídeo precisa ter origem em uma imagem fornecida por mim.**

Essa regra vale também para **sites e marcas de terceiros**, incluindo o site das Loterias Caixa: **não recriar, reconstruir ou inventar a aparência real de nenhum site que não tenha sido fornecido como imagem de referência.**

Sempre que uma cena mencionar "o site da Caixa" e nenhuma imagem de referência do site da Caixa tiver sido fornecida, não gerar essa interface. Representar a ação de forma abstrata (ex: a extensão do Jogos Bem Feitos preenchendo campos genéricos, sem replicar o layout, cores, logotipo ou identidade visual reais de nenhum site externo).

---

# 3. PRONÚNCIA OBRIGATÓRIA: TREVIN

O nome escrito do personagem é:

**Trevin**

Porém, atenção absoluta à pronúncia.

A pronúncia correta em português brasileiro é:

# tre-VIN

A sílaba tônica é:

# VIN

O nome vem de **Trevinho**.

Pronunciar exatamente como o começo de:

**Trevinho → tre-VIN-ho**

Portanto:

CORRETO:

**tre-VIN**

INCORRETO:

**TRÉ-vin**

Não pronunciar como nome inglês.

Não utilizar entonação estrangeira.

Não colocar a sílaba tônica em "Tre".

Sempre colocar a força da pronúncia em **VIN**.

Quando estiver escrito:

**"Eu sou o Trevin."**

a fala deve soar naturalmente em português brasileiro como:

**"Eu sou o tre-VIN."**

A representação fonética serve SOMENTE como instrução para geração do áudio. Nunca escrever "tre-VIN" em lugar nenhum.

**Não gerar nenhum texto, título, legenda ou closed caption na tela, de nenhum tipo, automático ou não.** O vídeo deve ficar totalmente livre de textos sobrepostos. O áudio é o único veículo das falas.

---

# 4. VOZ DO TREVIN

**Aviso prático:** o Veo 3 usa vozes fixas do Google (ex: Puck) e não permite escolher/desenhar um timbre customizado por texto: a descrição abaixo não vai mudar qual voz sai, só serve pra guiar a entonação/emoção dentro da voz que o modelo já usa (Puck tende a soar mais neutra/jovem, então funciona relativamente bem para um assistente de IA, mas não é garantido bater 100% com o descrito). Se a identidade sonora do Trevin precisar ser exata e consistente entre vídeos, a alternativa é gerar o vídeo sem depender da voz do Veo e **dublar por cima em pós-produção** com uma ferramenta de TTS que permita clonar/fixar uma voz própria (ex: ElevenLabs), sincronizando com a boca/movimento do Trevin.

Todo o áudio falado deve ser exclusivamente em:

# PORTUGUÊS BRASILEIRO (PT-BR)

Voz masculina brasileira, com timbre de **personagem/assistente de IA**, e não uma voz humana genérica de locução ou narração publicitária comum.

A voz deve ter uma leve textura tecnológica/sintética perceptível no timbre (não um efeito robótico exagerado, mas algo que deixe claro que quem fala é um assistente de IA, não um narrador humano comum).

A voz deve transmitir:

* inteligência;
* confiança;
* simpatia;
* domínio do produto;
* tecnologia;
* praticidade;
* leve descontração;
* identidade única de personagem (reconhecível, não intercambiável com qualquer voz masculina genérica).

Trevin deve soar como um **assistente inteligente que sabe o que está fazendo**, com um timbre que remeta à sua natureza de IA/mascote da marca.

**Nesta versão, o ritmo da fala precisa ser mais devagar e mais claro que numa peça de teaser rápido**, com pausas perceptíveis entre frases, como alguém explicando algo com calma para uma pessoa que está ouvindo pela primeira vez. Não apressar a locução para caber mais conteúdo; se uma frase não couber com folga no tempo da parte, é preferível encurtar a frase a acelerar a fala.

A voz deve ser natural e conversacional dentro dessa identidade, mas não robotizada ao ponto de soar sintetizada de forma grotesca, e também não uma voz humana comum de locutor.

Evitar interpretação excessivamente publicitária.

## NÃO USAR:

* voz humana genérica de locutor/narrador, sem nenhuma característica de personagem;
* voz infantil;
* voz de desenho animado;
* voz excessivamente fofa;
* voz robótica exagerada/caricata (tipo robô de filme antigo);
* voz caricata;
* sotaque estrangeiro;
* pronúncia inglesa;
* entusiasmo exagerado;
* fala apressada/corrida (regra nova desta versão: a v1 saiu rápida demais e ficou difícil de entender).

---

# 5. TRILHA E DESIGN DE SOM

Utilizar uma trilha instrumental:

* tecnológica;
* moderna;
* minimalista;
* sofisticada;
* dinâmica, mas discreta;
* jovem.

A música deve transmitir:

**tecnologia + inteligência + clareza + confiança.**

Começar discretamente e permanecer discreta durante toda a narração: o volume da trilha nunca pode competir com a voz do Trevin, especialmente porque agora ele fala mais devagar e em frases mais longas.

Pode ganhar um pouco mais de energia na Parte 4 (chamada para ação), mas sem virar uma "batida" que atropele o fim da fala.

Utilizar pequenos efeitos sonoros de interface nas transições entre telas, quando fizer sentido.

## NÃO UTILIZAR:

* música épica;
* música infantil;
* trilha de videogame;
* sons futuristas exagerados;
* cyberpunk;
* efeitos excessivos.

---

# 6. PARTE 1: GANCHO

## Duração: 0–3 segundos

**IMAGEM A USAR COMO FRAME INICIAL NESTA GERAÇÃO: foto do Trevin** (ver 0.2, image-to-video, não só "referência"; não redescrever a aparência do personagem no texto).

Começar imediatamente com uma composição visual forte, sem enrolação.

Mostrar a interface do **Jogos Bem Feitos** em um enquadramento elegante.

Trevin aparece em destaque integrado à interface.

**Utilizar exatamente o Trevin fornecido na imagem de referência.**

Não criar outro personagem.

Realizar uma aproximação muito sutil da câmera.

Trevin pode piscar ou realizar uma microanimação natural.

A abertura deve ser extremamente clean.

Poucos elementos.

Grande espaço visual.

### ÁUDIO:

Trevin fala:

**"Se você joga na loteria da Caixa, isso aqui vai te poupar um tempão."**

Tom direto, sem pressa: mesmo sendo o gancho, a frase não deve soar apressada.

Essa frase precisa segurar quem está passando o dedo, avisando de cara pra quem o vídeo é.

Dar uma pequena pausa no final antes de cortar para a Parte 2.

---

# 7. PARTE 2: INTRODUÇÃO (PRA QUEM É)

## Duração: 3–12 segundos

Trevin ainda não foi nomeado na Parte 1; aqui ele se apresenta e contextualiza o problema, em ritmo calmo, uma ideia de cada vez.

**IMAGEM A USAR COMO FRAME INICIAL NESTA GERAÇÃO: foto do Trevin** (ver 0.2). Se fizer sentido visualmente, pode-se compor Trevin com um fundo simples sugerindo "bagunça de apostador" (bilhetes, anotações), mas sem inventar tela de produto aqui, pois essa parte é sobre o problema, não sobre a solução.

Trevin é o narrador. Ele NÃO está conversando com o usuário nem respondendo perguntas: está explicando, olhando "para a câmera".

### ÁUDIO EXATO:

**"Eu sou o Trevin. Se você aposta na Mega-Sena, na Lotofácil ou em qualquer jogo da Caixa, sabe como é chato ficar montando jogo, conferindo número por número e organizando tudo na mão."**

Pronúncia obrigatória de "Trevin": **tre-VIN** (ver seção 3).

Falar em ritmo pausado, com uma pequena pausa depois de "Eu sou o tre-VIN" antes de continuar a frase, para dar tempo da apresentação "grudar" antes de emendar o resto.

---

# 8. PARTE 3: O QUE É O TREVIN / O PROJETO

## Duração: 12–24 segundos

Esta é a parte mais longa: Trevin explica o que ele é e o que faz, uma função por vez, cada uma acompanhada da tela correspondente do produto **parada tempo suficiente para ser lida** (mínimo 2–3 segundos por tela, nunca um flash rápido como na v1 anterior). Gerar em 4 trechos separados (um por função), cada um com a imagem de referência indicada, e no corte final encadear os 4 na ordem abaixo.

**Trecho A: "Eu sou a inteligência artificial do Jogos Bem Feitos" / "Eu gero seus jogos"** → usar a screenshot real da tela do Gerador como frame inicial (ver 0.2). São combinações numéricas de loteria (grades de números), nunca video game (ver 0.4). Mostrar o gerador funcionando, combinações sendo geradas dentro da interface, câmera parada ou com movimento mínimo para não distrair de entender a tela.

**Trecho B: "insiro direto na Caixa"** → sem screenshot real do site da Caixa fornecida; não usar imagem de site de terceiro, resolver de forma abstrata (ver regra 2.1). Mostrar a extensão do Jogos Bem Feitos em ação, preenchendo/inserindo jogos, aparecendo **dentro de um site genérico** como um painel/extensão lateral, nunca como aplicativo de celular.

**Trecho C: "organizo tudo separado por grupos"** → usar a screenshot real da tela de Meus Jogos como frame inicial (ver 0.2). Jogos aparecem organizados visualmente, com tempo suficiente na tela pra dar pra ler o agrupamento.

**Trecho D: "e ainda ajudo você a tocar bolão com os seus amigos"** → usar a screenshot real da tela de Jogadores/Apostas como frame inicial (ver 0.2). Mostrar jogadores, participações e saldos organizados, transmitindo controle simples do bolão.

### ÁUDIO EXATO (dividido nos 4 trechos, mas falado como uma sequência contínua e pausada, sem pressa):

**"Eu sou a inteligência artificial do Jogos Bem Feitos. Eu gero seus jogos, insiro direto na Caixa, organizo tudo separado por grupos e ainda ajudo você a tocar bolão com os seus amigos."**

Sincronizar visualmente cada tela com o trecho de fala correspondente. Cada troca de tela deve coincidir com uma pausa natural da fala, não cortar no meio de uma palavra.

---

# 9. REGRA CRÍTICA PARA AS TELAS DO PRODUTO

Caso sejam fornecidas imagens ou vídeos das telas reais do **Jogos Bem Feitos**, essas referências devem ser utilizadas como **fonte visual principal**.

**Nenhuma tela sem imagem de referência fornecida pode ser gerada** (ver regra 2.1). Se uma parte pede uma tela que não foi enviada, resolver a cena sem mostrar interface do produto.

Não reinterpretar completamente a interface.

Preservar:

* identidade visual;
* estrutura;
* componentes;
* cores;
* logotipo;
* organização;
* estilo;
* aparência geral.

Não inventar um dashboard futurista.

Não transformar o produto em um sistema genérico de IA.

Não criar telas de chatbot.

Não substituir a interface real por interfaces fictícias.

As telas devem parecer o **produto real em funcionamento**.

---

# 10. PARTE 4: CHAMADA PARA AÇÃO

## Duração: 24–30 segundos

**IMAGEM A USAR COMO FRAME INICIAL NESTA GERAÇÃO: foto do Trevin (ver 0.2).**

Depois da explicação das funcionalidades, diminuir o ritmo e voltar para uma composição clean, focada só em Trevin e na identidade visual do Jogos Bem Feitos.

Usar exatamente o mesmo Trevin apresentado anteriormente. Nenhuma mudança no personagem.

As funcionalidades apresentadas na Parte 3 podem aparecer discretamente ao fundo ou em pequenos recortes visuais, sem poluir a composição.

Entrada elegante do logotipo do Jogos Bem Feitos ao final.

**Não incluir nenhum ícone/logo de rede social (Instagram, TikTok ou qualquer outra) na composição.** O CTA deve ser comunicado somente pela fala, sem ícones de plataforma ou qualquer texto na tela.

### ÁUDIO:

Trevin fala:

**"Esse mês eu vou te mostrar cada uma dessas coisas de perto, uma por semana. Segue aqui pra não perder."**

Tom confiante e convidativo, sem pressa: a frase é mais longa que o CTA da v1 anterior, então precisa de tempo pra caber com folga dentro dos ~6 segundos da parte.

Essa parte deve transmitir claramente: **"isso foi só a introdução, o resto vem por aí."**

Finalizar com o logotipo perfeitamente legível.

---

# 11. DIREÇÃO VISUAL

O vídeo deve parecer um:

**TRAILER/APRESENTAÇÃO DE PRODUTO DIGITAL, EM RITMO DIDÁTICO.**

Não um comercial tradicional de loteria.

Não um desenho animado.

Não um vídeo infantil.

Não um vídeo genérico de IA.

Não um teaser picotado tipo "flash de features" (isso já foi tentado na v1 e ficou rápido demais para entender).

Referências conceituais:

* campanha moderna de SaaS;
* lançamento de aplicativo, com tempo de explicar;
* vídeo explicativo/onboarding de produto digital;
* motion design de startup;
* publicidade tecnológica minimalista;
* edição calma, mas ainda dinâmica nas transições de tela.

A estética deve transmitir:

**inteligência + organização + tecnologia + praticidade + confiança + clareza.**

Trevin é o fio condutor.

Mas:

# O PRODUTO É O PROTAGONISTA.

Trevin apresenta, explicando com calma.

As telas demonstram, com tempo suficiente para serem entendidas.

---

# 12. MOVIMENTAÇÃO

Utilizar movimentos discretos e profissionais:

* zoom suave;
* aproximação de câmera;
* pequenas mudanças de enquadramento;
* transições suaves entre telas (não cortes ultrarrápidos como na v1);
* movimentos de interface;
* microanimações;
* pequenos efeitos de profundidade.

Evitar movimentação excessiva.

A câmera não deve ficar constantemente se movimentando.

O vídeo precisa respirar: cada tela fica tempo suficiente para ser lida antes do próximo corte.

---

# 13. TEXTOS NA TELA

**Nenhum.** O vídeo não deve conter nenhum texto, título, legenda ou closed caption em momento algum, nem mesmo o nome do personagem. Toda a comunicação acontece por imagem, música e pela voz (mais devagar) do Trevin.

---

# 14. EVITAR ABSOLUTAMENTE

Não criar outro Trevin.

Não redesenhar Trevin.

Não reinterpretar o personagem.

Não transformar Trevin em 3D.

Não transformar Trevin em humano.

Não criar corpo para Trevin.

Não criar braços ou pernas.

Não infantilizar Trevin.

Não deixar Trevin excessivamente fofo.

Não criar estética Pixar.

Não criar estética de desenho infantil.

Não criar chatbot.

Não mostrar uma conversa de chat.

Não mostrar Trevin respondendo perguntas livremente.

Não criar hologramas.

Não criar estética cyberpunk.

Não usar excesso de neon.

Não usar excesso de partículas.

Não usar números de loteria voando pela tela.

Não representar "jogos" como video game, console, controle, pixel art ou tela de arcade: "jogos" é sempre combinação numérica de aposta de loteria (ver 0.4).

Não usar bolas de loteria flutuando.

Não usar moedas voando.

Não mostrar chuva de dinheiro.

Não mostrar pessoas comemorando prêmio.

Não criar elementos mágicos.

Não criar cenários fantasiosos.

Não criar interfaces futuristas fictícias.

Não criar aplicativo de celular para representar a extensão.

Não encher a tela de informações.

Não utilizar textos pequenos.

Não utilizar transições exageradas ou cortes ultrarrápidos (regra nova: nesta versão cada tela precisa de tempo pra ser entendida).

Não acelerar a fala do Trevin para caber mais conteúdo no tempo (regra nova: preferir encurtar o texto a acelerar a locução).

Não fazer promessas de ganhos.

Não sugerir aumento garantido das chances de ganhar.

Não incluir ícones ou logotipos de redes sociais (Instagram, TikTok ou qualquer outra) em nenhuma cena do vídeo.

Não adicionar nenhum texto, título, legenda ou closed caption na tela.

---

# 15. FALAS EXATAS

Não alterar, resumir, traduzir ou acrescentar palavras às falas.

Todo o áudio deve ser em **português brasileiro**.

### PARTE 1: GANCHO (0–3s)

**"Se você joga na loteria da Caixa, isso aqui vai te poupar um tempão."**

### PARTE 2: INTRODUÇÃO (3–12s)

**"Eu sou o Trevin. Se você aposta na Mega-Sena, na Lotofácil ou em qualquer jogo da Caixa, sabe como é chato ficar montando jogo, conferindo número por número e organizando tudo na mão."**

Pronúncia de "Trevin": **tre-VIN**

### PARTE 3: O QUE É O TREVIN / O PROJETO (12–24s)

**"Eu sou a inteligência artificial do Jogos Bem Feitos. Eu gero seus jogos, insiro direto na Caixa, organizo tudo separado por grupos e ainda ajudo você a tocar bolão com os seus amigos."**

### PARTE 4: CHAMADA PARA AÇÃO (24–30s)

**"Esse mês eu vou te mostrar cada uma dessas coisas de perto, uma por semana. Segue aqui pra não perder."**

---

# 16. VERIFICAÇÃO FINAL OBRIGATÓRIA

Antes de gerar o resultado, garantir:

1. O personagem utilizado é visualmente consistente com a imagem do Trevin fornecida, incluindo as mesmas cores, sem nenhuma alteração.
2. Nenhum novo mascote foi criado.
3. Nenhuma tela do sistema aparece sem ter sido fornecida como imagem de referência (ver regra 2.1).
4. O nome Trevin é pronunciado **tre-VIN**, com força na última sílaba.
5. Todo o áudio está em português brasileiro.
6. Trevin possui voz com timbre de personagem/assistente de IA, e não uma voz humana genérica de locutor (ver seção 4).
7. A fala está em ritmo pausado e claro em todas as 4 partes, sem trechos apressados (regra nova desta versão).
8. Cada tela do produto na Parte 3 permanece visível tempo suficiente para ser lida (mínimo 2–3s), sem flashes rápidos.
9. O produto aparece mais do que o mascote.
10. A extensão aparece como extensão dentro do site, e não como celular.
11. Não existe conversa de chatbot.
12. O vídeo possui aparência profissional de campanha de SaaS, agora em tom explicativo/didático.
13. O vídeo permanece clean e não fica visualmente poluído.
14. As interfaces fornecidas como referência são preservadas.
15. O vídeo termina com Trevin, Jogos Bem Feitos e o CTA para seguir.
16. Nenhum ícone ou logotipo de rede social aparece em qualquer cena.
17. Nenhum site ou marca de terceiros (incluindo Caixa) foi recriado sem imagem de referência fornecida.
18. Não existe absolutamente nenhum texto, título, legenda ou closed caption na tela em nenhum momento do vídeo.
19. Cada parte/trecho foi gerado usando a imagem certa (Trevin ou screenshot) como frame inicial (ver 0.2), nunca só como referência de estilo.
20. Nenhuma tela mostra jogos eletrônicos, consoles, controles ou pixel art: "jogos" aparece sempre como combinações numéricas de loteria (ver 0.4).
21. A duração total fica em torno de 30 segundos, distribuída nas 4 partes (0–3s, 3–12s, 12–24s, 24–30s).
