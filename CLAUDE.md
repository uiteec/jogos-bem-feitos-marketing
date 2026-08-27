# Regras do projeto — Jogos Bem Feitos Marketing

Estas regras têm prioridade sobre qualquer comportamento padrão. Ver também `README.md` para a estrutura de pastas.

## Conteúdo e voz

- **Trevin é o centro de todo conteúdo.** Todo material de marketing (reels, carrosséis, posts, anúncios) deve girar em torno do Trevin, a IA/mascote do produto, de preferência na voz dele (1ª pessoa). Ver `contexto/trevin.md`.
- Antes de criar qualquer peça, consultar `contexto/produto.md` para garantir que a mensagem está alinhada com o que o produto realmente entrega.
- Cuidado editorial: nunca sugerir promessa de prêmio, enriquecimento ou garantia de resultado. Ver as seções "Cuidado editorial" de cada peça de reel/carrossel para riscos específicos (ex.: linguagem de extensão Chrome, confirmação de resgate de prêmio).

## Escrita e formatação

- **Sempre usar a skill `humanizer-pt-br`** ao criar ou revisar qualquer texto do projeto (roteiro, legenda, descrição de postagem, copy de anúncio, texto de slide). Ela remove traços de escrita gerada por IA (linguagem promocional, estruturas mecânicas, conectivos em excesso, frases de preenchimento, aspas tipográficas, etc.) e é o mecanismo padrão para garantir que o texto soe humano antes de ser entregue.
- **Nunca usar travessão "—" (em dash)** em nenhum texto do projeto (roteiro, legenda, prompt, descrição de postagem, documentação). É um tique reconhecível de texto gerado por IA. Trocar por vírgula, ponto final, "e"/"ou"/"mas", dois pontos ou parênteses, conforme o que soar mais natural em português. Nunca usar hífen simples "-" como substituto direto no meio de frases (hífen simples só vale em compostos ou intervalos de data já existentes, ex.: "05-09").
- **Sempre criar arquivos em `.md`**, mesmo para texto puro (falas, roteiros, narração). Nunca criar `.txt`.
- Quando o usuário pedir "texto pronto pra copiar", entregar um único bloco de código com todo o conteúdo (legenda + CTA + hashtags), não seções separadas por título que exigem copiar pedaço por pedaço.

## Design de carrossel (Instagram)

Regras que valem tanto para o template-base (`prompts-base/feed/prompt-feed-carrossel.md`) quanto para qualquer `prompts/slideN.md` de carrossel específico em `planejamento/social/2026/*/carrossels/`.

**Prompts de slide de carrossel devem ser CURTOS** (dezenas de linhas, não centenas). Um prompt longo e cheio de palavras soltas de branding ("inteligência", "praticidade", "segurança", "estratégia", "check", "análises" etc., mesmo quando usadas só como adjetivo de personalidade em alguma seção distante) faz a IA de geração de imagem transformar essas palavras em cards, ícones, checklists e badges que ninguém pediu. Isso já aconteceu duas vezes seguidas neste projeto: a primeira correção (só pedir "Trevin pequeno" e proibir alguns itens) não resolveu porque o prompt continuava enorme; só resolveu de fato depois de reescrever os arquivos como prompts diretos e curtos, com só os elementos permitidos listados explicitamente. Ver `feedback_carrossel_slides_secundarios.md` na memória para o histórico completo.

O **slide 1** é a capa: pode ter título + texto secundário menor, Trevin em destaque (até metade da imagem) e logotipo.

**A partir do slide 2**, em todo carrossel, a imagem tem SOMENTE 3 elementos (ou 4, se houver CTA): a frase, o Trevin pequeno, o indicador de página, e opcionalmente um CTA curto. Nada além disso:

1. **Trevin pequeno** — no máximo ~1/4 da imagem, pose simples, sem segurar nada e sem nenhum elemento ao redor dele.
2. **Uma única frase, em tamanho único** — nunca "título grande + texto complementar/secundário menor".
3. **Sem logotipo** nos slides 2+ (só o slide 1 tem logo).
4. **Nenhum elemento gráfico extra**: nada de dezenas, números de loteria, cartões, ícones, indicadores, gráficos, checklists, pranchetas/celulares na mão do Trevin, ou qualquer fileira de mini-cards/badges.

Ao escrever o prompt, listar explicitamente "esta imagem tem SOMENTE N elementos" e depois repetir a lista de proibições relevantes logo abaixo do conteúdo (não só numa seção genérica distante) — isso reduz a chance da IA de imagem "aproveitar" palavras do resto do documento.

## Memória

Este projeto usa memória persistente entre conversas (`~/.claude/projects/.../memory/`). Antes de assumir que algo aprendido numa conversa anterior ainda é válido, verificar o estado atual dos arquivos/código — a memória pode estar desatualizada.
