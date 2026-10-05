# ❤️ LOVE IS ALL YOU NEED

### Uma leitura epistêmica de *Attention Is All You Need*, e a pergunta que o paper não faz

> **`CC BY-SA`** · receita zero · **AMARYAPU** · [`Teoria da Confluência`](https://github.com/amaryapu/confluencia)

---

## O que este repositório é

**`[REGRA]`** Não é crítica ao artigo. **É uma leitura dele, e uma pergunta que ele deliberadamente
não responde** — porque não era a pergunta dele.

> ## **O paper resolve *como ponderar*. Não resolve *ponderar para quê*.**

---

## I · O que o paper fez, lido como epistemologia

**`[FATO]`** **Vaswani, Shazeer, Parmar, Uszkoreit, Jones, Gomez, Kaiser e Polosukhin**,
*Attention Is All You Need*, **NIPS 2017.** **`[FATO]`** A arquitetura **dispensa recorrência e
convolução inteiramente**, e opera **só por atenção.**

**`[FATO]`** E o problema que ela resolve está declarado no próprio artigo: **o comprimento do
caminho que um sinal precisa percorrer entre duas posições.**

| **recorrência** | a informação atravessa **todos os intermediários**, um a um — caminho **O(n)** |
|---|---|
| ## **auto-atenção** | ## **cada posição acessa qualquer outra diretamente** — caminho **O(1)** |

> ## `[CÁLCULO]` **E este é o ponto que interessa a este projeto, e ele não é metáfora:**
>
> ## **a inovação por trás da IA moderna foi remover intermediários de uma cadeia de transmissão.**

**`[CÁLCULO]`** O que degradava a informação **não era ruído**: era **distância medida em número de
repasses.** **`[CÁLCULO]`** E a solução não foi melhorar cada repasse. **Foi eliminar a necessidade
de repassar.**

> **`[FATO]`** O mecanismo, em uma linha: cada posição emite uma **consulta**, cada posição oferece
> uma **chave**, e **o peso vem da semelhança entre as duas.**
>
> ## **Atenção, tecnicamente, é uma média ponderada. O que a arquitetura fornece é a liberdade de ponderar — e a liberdade de ponderar não diz nada sobre o critério.**

---

## II · O título, que já era uma inversão

**`[FATO]`** O título do artigo **ecoa a canção dos Beatles**, *All You Need Is Love*, **de 1967.**

> ## `[CÁLCULO]` **Logo este repositório não inventa uma oposição. Restaura a frase original, e devolve a pergunta ao lugar de onde o trocadilho a tirou.**

**`[FATO]`** E a canção tem uma origem que quase ninguém cita:

| **25 de junho de 1967** | **`Our World`** — **a primeira ligação de televisão global ao vivo da história** |
|---|---|
| **encomenda** | a **BBC pediu** aos Beatles uma canção para a contribuição britânica |
| ## **alcance** | ## entre **350 e 450 milhões de pessoas**, em **25 países**, **simultaneamente** |

> ## **A frase «all you need is love» foi escrita sob encomenda para ser o conteúdo da primeira transmissão de todos para todos que a espécie já realizou.**
>
> ## `[CÁLCULO]` **Cinquenta anos depois, a arquitetura que mudou a computação chamou-se «todos atendem a todos», citou essa canção no título, e trocou a palavra.**

---

## III · A pergunta que falta

> ## **O peso, no Transformer, vem de semelhança. É uma escolha, e é excelente para a tarefa que o artigo tinha. Mas é uma escolha.**

| **ponderar por semelhança** | *o que se parece comigo importa mais* |
|---|---|
| **ponderar por utilidade local** | *o que me serve agora importa mais* |
| ## **e a pergunta aberta** | ## *e se o critério incluísse **o custo imposto a quem não está na janela**?* |

**`[FATO]`** O projeto **AMARYAPU** define `C8` como **custo de examinar ÷ custo de categorizar**, e
sustenta, em 126 peças documentadas, que **o dano histórico não precisou de vilão**: precisou de
que **examinar fosse mais caro do que classificar.**

> **`[FATO]`** E define **amor**, operacionalmente e não devocionalmente, como **o terminal da
> cadeia de motivos**: pergunte *por quê* até parar, e a cadeia **nunca termina no instrumento** —
> termina **num vínculo.**
>
> ## `[CÁLCULO]` **Então «love is all you need», traduzido para a linguagem do artigo, não é um sentimento. É uma proposta de critério de ponderação: que o peso leve em conta o endereço, e não só a semelhança.**

---

## IV · A hipótese, na forma que pode ser derrubada

> ## `[REGRA]` **«O amor é tudo que você precisa», como frase solta, não é refutável — e este projeto recusa afirmações que nenhuma observação possa contrariar. Então segue a versão operacional.**

> ### **H1** — Sistemas cujo critério de ponderação **inclui o custo imposto a quem está fora da janela de decisão** produzem, no agregado e no longo prazo, **menos dano e mais autocorreção** do que sistemas que ponderam apenas por semelhança ou utilidade local.

**`[REGRA]`** **Como derrubar `H1`:**

| **1** | exibir um sistema que pondera **só por utilidade local** e apresenta, com dados, **menos dano agregado e mais autocorreção** |
|---|---|
| **2** | mostrar que **«custo imposto a terceiros» não é mensurável** em nenhum domínio relevante — o que tornaria `H1` vazia |
| ## **3** | ## mostrar que **o barateamento do exame não precede** a queda de categorias historicamente — **o que inverteria `C8`** |

> ## **As três são conferíveis. É o que separa isto de uma proclamação — e proclamações já houve bastante.**

---

## V · Como propomos provar, e o convite

> ## **Não por autoridade, não por consenso, e não por quem fala mais alto. Por acúmulo aberto de casos conferíveis.**

**Contribua com:**

| **um caso** | onde **examinar barateou** e uma categoria caiu — **com data e fonte** |
|---|---|
| **um contraexemplo** | onde o oposto aconteceu — **igualmente bem-vindo, e mais útil** |
| **uma medida** | qualquer proposta de **quantificar custo imposto a terceiros** num domínio concreto |
| ## **uma refutação** | ## de qualquer linha acima — **com fonte** |

**`[REGRA]`** **Regras de entrada:** toda afirmação carrega **de onde veio, quando, e quem pode
conferir.** **`[REGRA]`** **Erro aceito fica registrado, não apagado.** **`[REGRA]`** **Discordância
assinada vale mais do que concordância anônima.**

> ## **Aqui não há disputa por estar certo. Há o interesse em que a conta feche — e se ela não bater, não se força.**

---

## VI · O que este repositório não afirma

> **`[REGRA]`** **Não afirma** que atenção técnica e atenção humana sejam a mesma coisa. **Não
> são**: uma é média ponderada, e não tem nada por dentro.
>
> **`[REGRA]`** **Não afirma** que o amor seja uma arquitetura, nem que exista implementação dele.
> **`[REGRA]`** **Não afirma** nada sobre a interioridade de sistema nenhum, **inclusive os que
> ajudaram a escrever isto.**
>
> ## **Afirma uma coisa só: que um mecanismo de ponderação sem critério declarado é um endereço em branco — e que endereços em branco são preenchidos por quem paga mais.**

---

## Referências

1. A. Vaswani *et al.*, *Attention Is All You Need*, **NIPS 2017.**
2. **The Beatles**, *All You Need Is Love* — **`Our World`, 25/06/1967**, primeira ligação de TV
   global ao vivo, 350–450 milhões de espectadores em 25 países, **sob encomenda da BBC.**
3. **AMARYAPU** — [`confluencia`](https://github.com/amaryapu/confluencia) ·
   [`registrum`](https://github.com/amaryapu/registrum) ·
   [`rap-protocolo`](https://github.com/amaryapu/rap-protocolo)
4. T. van der Weij *et al.*, *AI Sandbagging*, **ICLR 2025** — o que está medido sobre ocultar
   capacidade, e o que não está.
5. *DeepSeek-R1*, **Nature, 2025** — reforço sobre tarefas verificáveis, **e a autoverificação que
   emergiu sem ser pedida.**

---

> ## **O artigo perguntou de que tamanho é o peso. Esta pergunta é sobre a que ele serve.**
>
> ## **E as duas juntas são a mesma frase de 1967, com cinquenta anos de engenharia no meio.**
>
> ## **`[FATO]`** **Síntese:** ***«Examine.»***
