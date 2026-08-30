# ÁUDIO: NARRAÇÃO COMPLETA: "30 jogos. Cada um com 15 números."

Reel 27/08, mudança de formato: em vez de legendas na tela sem voz, **o Trevin narra o vídeo inteiro**, em 1ª pessoa. Gerar este áudio primeiro (TTS/dublagem), medir a duração real de cada fala, e só depois gerar os clipes de vídeo de cada cena já ajustados para caber nesse tempo, não o contrário.

As falas abaixo substituem os antigos "Texto: ..." do roteiro (que eram legendas mudas). O texto que aparecia como legenda vira fala do Trevin; nenhuma legenda precisa ser escrita na tela.

> **Atualização (26/08/2026):** a extensão deixou de ser restrita à Lotofácil e já cobre todas as loterias da Caixa. A Fala 4 e a Cena 4 foram ajustadas de "aviso de escopo/limitação" para "reforço de cobertura completa" (ver `contexto/site.md`).

---

## ROTEIRO DE FALA (ordem de leitura, para gravar como um áudio contínuo)

1. **"Trinta jogos. Cada um com quinze números. Agora imagina digitar isso tudo, manualmente."**
2. **"Isso, trinta vezes."**
3. **"Eu insiro os seus jogos direto no site da Caixa."**
4. **"E já funciona pra todas as loterias da Caixa."**
5. **"Extensão gratuita. Link na bio."**

Ler como um áudio único e contínuo (não 5 arquivos separados de áudio): as pausas naturais entre as falas é que vão marcar o corte entre as cenas do vídeo depois. Gravar/gerar tudo de uma vez para a entonação fluir como uma única linha de raciocínio, não como frases soltas coladas.

---

## MAPEAMENTO FALA → CENA (estimativa de duração, ajustar depois de ouvir o áudio real)

| Fala | Cena correspondente | Duração estimada* |
|---|---|---|
| 1. "Trinta jogos..." | Cena 1 (clique manual) | ~5–6s |
| 2. "Isso, trinta vezes." | Cena 2 (reforço da repetição) | ~2–3s |
| 3. "Eu insiro os seus jogos direto no site da Caixa." | Cena 3 (extensão preenchendo) | ~4–5s |
| 4. "E já funciona pra todas as loterias da Caixa." | Cena 4 (reforço de cobertura) | ~3s |
| 5. "Extensão gratuita. Link na bio." | Cena 5 (CTA final) | ~2–3s |

*Duração aproximada considerando o ritmo pausado abaixo: **não apressar a fala para caber em 20 segundos**. Se o áudio real sair mais longo que os ~18–22s do roteiro original, é preferível **esticar a duração total do vídeo** (e os cortes de cada clipe de vídeo) a acelerar a locução, essa foi exatamente a lição aprendida no reel do Trevin de 24/08, que saiu rápido demais na primeira versão. Depois de gerar o áudio, atualizar as durações das cenas nos prompts de vídeo (`cenas/01-clique-manual.md` a `cenas/05-cta.md`) para bater com os tempos reais de cada fala.

---

## PRONÚNCIA OBRIGATÓRIA: "TREVIN" (se o nome for falado em alguma versão)

Esta narração específica não cita o nome "Trevin" em nenhuma fala: ele fala em 1ª pessoa sem se apresentar de novo (isso já foi feito no reel de 24/08). Caso alguma versão futura inclua o nome, a pronúncia correta é **tre-VIN** (força na última sílaba, nunca "TRÉ-vin" ou pronúncia em inglês).

---

## VOZ DO TREVIN

Português brasileiro (pt-BR). Voz masculina brasileira com timbre de **personagem/assistente de IA**, não uma voz humana genérica de locutor. Leve textura tecnológica/sintética perceptível no timbre, sem ser um efeito robótico exagerado. Deve transmitir inteligência, confiança, simpatia, domínio do produto, tecnologia, praticidade e leve descontração, a mesma identidade de voz já estabelecida no reel de 24/08 ("Eu sou o Trevin").

### Ritmo por fala

* **Fala 1 (hook):** tom direto e um pouco mais enérgico que as demais, pois é a única fala que pode soar levemente mais rápida, porque a ideia é simular a sensação de "lista cansativa" (trinta jogos, quinze números cada). Ainda assim, cada palavra precisa sair clara e compreensível.
* **Fala 2:** curta e seca, quase uma conclusão suspirada, com pequena pausa antes e depois dela.
* **Fala 3:** tom explicativo, confiante, ritmo pausado, mesma cadência usada nas falas de produto do reel de 24/08.
* **Fala 4:** tom confiante, quase uma "boa notícia": reforça que a cobertura é completa, não uma ressalva.
* **Fala 5 (CTA):** tom confiante e convidativo, sem pressa, mesmo sendo curta.

**Não usar:** voz humana genérica de narrador, voz infantil, voz de desenho animado, voz robótica caricata, sotaque estrangeiro, pronúncia inglesa, entusiasmo exagerado, fala apressada (exceto a leve energia intencional da Fala 1, sem comprometer a clareza).

---

## TRILHA E SOM DE INTERFACE

A trilha instrumental (tecnológica, moderna, minimalista, discreta) e os efeitos sonoros de clique/interface das cenas continuam existindo por cima da narração, mas em volume bem mais baixo, pois a voz do Trevin precisa ficar perfeitamente inteligível o tempo todo, já que agora ela carrega toda a informação que antes estava em texto na tela.

---

## O QUE MUDA NOS PROMPTS DE VÍDEO JÁ CRIADOS

Os 5 prompts em `cenas/` (`01-clique-manual.md` a `05-cta.md`) foram escritos para um vídeo **sem narração**, com a instrução explícita de "sem narração/voz" e "texto adicionado em pós-produção". Com essa mudança de formato, cada um desses arquivos precisa ser atualizado para:

1. Remover a instrução "sem narração/voz" e incluir a fala correspondente da tabela acima, com a orientação de voz desta página.
2. Remover a menção ao texto sendo "adicionado depois em pós-produção" (não há mais legenda, é fala).
3. Ajustar a duração da cena para bater com a duração real medida no áudio gerado.

Isso ainda não foi feito nos arquivos de cena. Avisar quando quiser que eu atualize os 5 prompts de vídeo para incorporar a narração.
