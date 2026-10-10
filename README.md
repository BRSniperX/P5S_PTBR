# Tradução PT-BR de Persona 5 Strikers — v2.2

<img width="2048" height="768" alt="persona5_strikers_nexus_traducao_ptbr_sem_duplicacao" src="https://github.com/user-attachments/assets/23c654c3-d7cc-477f-9160-25ab8ebf6b5c" />

Tradução para português do Brasil de **Persona 5 Strikers** (PC / Steam - Switch/Emulador).
Texto e interface gráfica, completos.

**Esta versão é só de arte: a interface gráfica foi refeita.** O texto não
mudou.

> **Já está na v2.1?** É só copiar por cima, aceitando substituir — são os
> mesmos três arquivos. **Vindo da v2.0.1 ou anterior?** Leia «Vindo da v2.0,
> v2.0.1 ou anterior» antes de copiar.

---

## O que mudou

### A arte da interface, refeita

Na v2.1, parte das imagens traduzidas usava letras de fontes genéricas, que
destoavam do resto do jogo. Na v2.2 a interface gráfica foi refeita, imagem por
imagem, para parecer uma tradução oficial.

- **A letra vem do próprio jogo.** Na grande maioria das imagens, cada letra é
  recortada de onde o jogo já a desenhou — nas outras versões de idioma da
  mesma imagem, ou em outra imagem da mesma família de letra — com o contorno,
  a sombra, o papel recortado e a inclinação do original.
- **Algumas artes de destaque foram redesenhadas à mão** no estilo do
  original, onde as letras do jogo não davam conta: os três MISSÃO, MANDOU
  BEM, ATAQUE TOTAL e OBTIDO!!.
- **O menu inicial foi redesenhado** — NOVO JOGO, CARREGAR JOGO, PRESSIONE
  QUALQUER BOTÃO e os demais itens — no estilo de bilhete recortado do
  original. O selo agora mostra **PT-BR v2.2**.
- **Imagens que todos os idiomas oficiais deixavam em japonês** agora estão em
  português, no estilo do jogo.
- **Telas de missão e de batalha** — MISSÃO, MANDOU BEM, SUBIU DE NÍVEL,
  ATAQUE TOTAL, OBTIDO!!, FALAR e os outros avisos — com as letras e as
  sombras de fundo acompanhando o texto, como no original.
- **Os avisos de ação** (MOVER!, ROUBAR, EXAMINAR...) não encostam mais no
  ícone do botão.
- **Compressão melhor.** O formato de textura do jogo mancha blocos que
  misturam cores muito diferentes (vermelho e branco, por exemplo). As
  imagens novas passam por um ajuste que evita isso.

Das 23 texturas de interface, **19 mudaram** e **4 são byte a byte idênticas**
à v2.1. O arquivo de texturas tem 9,29 MB (era 9,11 MB): foi recompactado, sem
espaço morto — o aumento é só das imagens novas. O download tem **65,6 MB**.

### O texto não mudou

O `LINKDATA.BIN` é **byte a byte idêntico** ao da v2.1. Isso foi conferido, não
suposto. A tradução está fechada desde a revisão integral da v2.0: 23.933
falas, cada uma lida no contexto da cena em que aparece.

### Continua sem nenhum arquivo de terceiros

Como na v2.1, o pacote **não traz** `dinput8.dll` nem HexPatcher: não há DLL
injetada, não há `.asi`, não há script, e o executável do jogo **não é
modificado**. São quatro arquivos: três de dados do jogo e um LEIA-ME. Quem usa
o **P5StrikersFix** ou outro mod com carregador próprio não precisa conferir
nada antes de copiar.

---

## Instalação

**Esta versão substitui dois arquivos do jogo.**

### 1. Faça backup dos dois arquivos

```
P5S\data\pd_ww\LINKDATA.BIN
P5S\data\motor_rsc\ScreenLayout.rdb
```

Esqueceu ou perdeu a cópia? Não tem problema: a verificação de integridade da
Steam baixa os originais de volta.

### 2. Deixe o jogo em ESPANHOL — obrigatório

A tradução **substitui os arquivos do idioma espanhol**. Ela não adiciona um
idioma novo: reescreve o espanhol em português.

**Jogar em outro idioma com a tradução instalada quebra o jogo** — a interface
fica corrompida, com texto ilegível, embaralhado ou fora do lugar.

Steam → botão direito em *Persona 5 Strikers* → **Propriedades** → **Idioma** →
**Espanhol**. Espere a Steam baixar os arquivos do idioma. **Só então** instale.

### 3. Copie a pasta `data` do pacote para dentro da pasta do jogo

```
P5S\data\pd_ww\LINKDATA.BIN                      (substitui)
P5S\data\motor_rsc\ScreenLayout.rdb              (substitui)
P5S\data\motor_rsc\ScreenLayout.rdb.bin_9        (substitui, ou arquivo novo)
```

A pasta do jogo normalmente fica em `...\Steam\steamapps\common\P5S`.
Na Steam: botão direito no jogo → **Gerenciar** → **Procurar arquivos locais**.

### 4. Abra o jogo

O menu inicial deve aparecer em português, com o selo **PT-BR v2.2** embaixo do
logo.

---

## Vindo da v2.1

Copie por cima, aceitando substituir. Não há nada para apagar.

## Vindo da v2.0, v2.0.1 ou anterior

**Apague os arquivos do método antigo**, senão os dois ficam convivendo e o
antigo vence:

```
P5S\dinput8.dll
P5S\update\HexPatcher.asi
P5S\update\HexPatcher.ini
P5S\update\data\pd_ww\LINKDATA.BIN
P5S\update\data\pd_ww\LINKDATA.IDX
P5S\update\data\motor_rsc\ScreenLayout.rdb
P5S\update\data\motor_rsc\ScreenLayout.rdb.bin_9
```

> **Usa o P5StrikersFix?** Então **não apague o `dinput8.dll`** — ele é o
> carregador que o P5StrikersFix também usa. Apague só os `HexPatcher.*` e o
> conteúdo de `update\data\`. A tradução não depende dele, e os dois convivem
> sem conflito.

---

## A Steam desfaz a instalação

Como a tradução substitui arquivos do jogo, **a verificação de integridade da
Steam devolve os originais** e a tradução desaparece. O mesmo vale se o jogo
receber uma atualização. Não é defeito, é como a Steam funciona — quando
acontecer, copie os arquivos outra vez.

### Para desinstalar

Devolva os dois arquivos do seu backup e apague o
`data\motor_rsc\ScreenLayout.rdb.bin_9`, que não existe no jogo original.

Sem backup? Rode a verificação de integridade na Steam e depois apague o
`.bin_9` na mão.

---

## Não funcionou?

| O que você vê | Causa quase certa |
|---|---|
| Texto **embaralhado** ou ilegível | O idioma na Steam não está em espanhol. É de longe a causa mais comum. |
| Jogo em **espanhol**, nada em português | Os arquivos não foram para a pasta certa. Confira a lista caminho por caminho. |
| Texto em português, **imagens em espanhol** | Faltou o `ScreenLayout.rdb.bin_9`, ou o `ScreenLayout.rdb` não foi substituído. |
| Selo ainda diz **v2.1** | O `ScreenLayout.rdb` ou o `.bin_9` não foi substituído. Copie de novo, aceitando substituir. |
| Português **sumiu** depois de um tempo | A Steam verificou ou atualizou o jogo. Copie os arquivos de novo. |
| Interface **esticada** em ultrawide | Não é a tradução. É o jogo, e quem conserta é o **P5StrikersFix**, que não vem aqui e nunca veio. |
| Jogo **não abre** | Restaure os dois arquivos do backup e reporte o problema. |

---

## O que está traduzido

**Texto** — completo e revisado linha a linha: diálogos, menus, itens,
habilidades, descrições, solicitações, tutoriais e as legendas dos vídeos.

**Interface gráfica** — completa. No Persona 5 Strikers, boa parte da interface
**não é texto**: são imagens desenhadas, no estilo recortado da série. Trocar uma
palavra ali significa redesenhar a imagem, reproduzindo a letra, o contorno, a
sombra e a inclinação do original.

## O que ficou de fora, de propósito

- **Placas e cartazes do cenário** (farmácia, estação, lojas de rua). Ficam em
  japonês, como no jogo original — nem a localização oficial em espanhol as
  traduziu. Traduzir quebraria a ambientação de Tóquio.
- As **168 capturas de tutorial** e o **aviso legal em japonês da abertura**.

---

## Sobre «o último patch»

A v2.1 foi anunciada como provavelmente o último patch. A v2.2 veio porque a
arte ainda podia ficar mais perto do original — o texto continua fechado, e
nada aqui muda o que você lê.

O projeto segue em manutenção: **bug reportado continua sendo corrigido**. Se
você encontrar qualquer coisa, mande um print e o nome da tela.

---

## Créditos e avisos

- Tradução PT-BR: trabalho independente, sem vínculo com Atlus, SEGA ou
  Koei Tecmo.
- Agradecimento a **Ahtheerr** e **OTTYSS**.
- *Persona 5 Strikers* © ATLUS © SEGA / © KOEI TECMO GAMES. Todos os direitos
  reservados. Este é um projeto de fã, gratuito e sem fins lucrativos.
