# Tradução PT-BR de Persona 5 Strikers — v2.1


Tradução para português do Brasil de **Persona 5 Strikers** (PC / Steam).
Texto e interface gráfica, completos.

**Esta versão não contém nenhum arquivo de terceiros.** É a mudança principal, e
ela é estrutural.

> **⚠️ Atualizando da v2.0 ou v2.0.1? A instalação mudou.** Apague os arquivos
> antigos antes de copiar os novos (`dinput8.dll`, `HexPatcher.*` e o conteúdo de
> `update\data\`), senão os dois métodos convivem e o antigo vence. Detalhes em
> «Vindo da v2.0, v2.0.1 ou anterior». *Usa o P5StrikersFix? Não apague o
> `dinput8.dll` — leia a seção antes.*

---

## O que mudou

### Nenhum componente de terceiros, nenhum script

Até a v2.0.1, o pacote precisava de duas peças que não eram nossas:

- o **Ultimate ASI Loader** (`dinput8.dll`), que injetava código no processo do
  jogo e interceptava as chamadas de abertura de arquivo do Windows
  (`CreateFileA/W`, `FindFirstFileA/W`, `GetFileAttributesW`);
- o **HexPatcher** (`HexPatcher.asi`), que reescrevia em memória a tabela de
  índice dos textos.

**Nenhuma das duas vem mais.** Não há DLL injetada, não há `.asi`, não há gancho
em API do Windows, não há script, e o executável do jogo **não é modificado**.

O pacote agora tem **quatro arquivos**: três de dados do jogo e um LEIA-ME.

### Por que isso só foi possível agora

A tabela que diz onde cada bloco de texto começa dentro do arquivo de dados **não
é um arquivo**: ela está dentro do próprio executável do jogo. Era por não saber
disso que o projeto usava o HexPatcher — ele reescrevia essa tabela em tempo de
execução, porque o texto do mod que serviu de base ao projeto tinha ficado
**maior** que o original e precisava de endereços novos.

O nosso texto em português **não fica maior**. Nos 332 blocos que a tradução
toca, ele termina mais curto que o espanhol original — a folga vai de 4 bytes a
quase 9 KB. Então cada bloco traduzido entra exatamente no lugar do original, com
o mesmo tamanho, e a tabela que já está no executável continua valendo sem uma
única alteração.

### O que isso muda na prática

- **Se der problema, o problema é nosso.** Não há mais como uma peça de terceiro,
  numa versão antiga ou em conflito com antivírus, entrar na conta.
- **Convive com qualquer outro mod.** Como o pacote não traz `dinput8.dll`, ele
  não tem como sobrescrever o de ninguém. Quem usa o **P5StrikersFix** ou outro
  mod com carregador próprio não precisa mais conferir nada antes de copiar.
- **Nada externo carregado junto com o jogo.**

### Também nesta versão

- **O selo do menu inicial** agora mostra **PT-BR v2.1**.
- **O `OBTIDO!` foi refeito** — a arte que aparece ao receber um item.
- **A arte ficou 2,81 MB menor** (11,91 MB → 9,11 MB, 24% menos). O arquivo de
  texturas guardava espaço morto de versões anteriores; foi recompactado **sem
  recomprimir nenhuma imagem**. As 23 texturas foram conferidas uma a uma e
  descomprimem idênticas às da v2.0.1 — não há perda de qualidade.
- O download caiu de 69,9 MB para **65,8 MB**.

### O texto não mudou

**Os 332 blocos de texto são byte a byte idênticos aos da v2.0.1.** Isso foi
conferido, não suposto. A tradução está fechada desde a revisão integral da v2.0:
23.933 falas, cada uma lida no contexto da cena em que aparece.

Das 23 texturas de interface, **21 são byte a byte idênticas** à v2.0.1. As duas
que mudaram são o selo e o `OBTIDO!`.

---

## Instalação

**Atenção: esta versão substitui dois arquivos do jogo.** As anteriores não
faziam isso — elas punham tudo numa pasta `update\` separada.

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
P5S\data\motor_rsc\ScreenLayout.rdb.bin_9        (arquivo novo)
```

A pasta do jogo normalmente fica em `...\Steam\steamapps\common\P5S`.
Na Steam: botão direito no jogo → **Gerenciar** → **Procurar arquivos locais**.

### 4. Abra o jogo

O menu inicial deve aparecer em português, com o selo **PT-BR v2.1** embaixo do
logo.

---

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
> conteúdo de `update\data\`. A tradução nova não depende dele, e os dois
> convivem sem conflito.

---

## A Steam desfaz a instalação

Como esta versão substitui arquivos do jogo, **a verificação de integridade da
Steam devolve os originais** e a tradução desaparece. O mesmo vale se o jogo
receber uma atualização. Não é defeito, é como a Steam funciona — quando
acontecer, copie os arquivos outra vez.

Isso foi testado: a verificação repõe os dois arquivos substituídos, **não toca
no executável** e **não apaga** o `ScreenLayout.rdb.bin_9`.

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
| Português **sumiu** depois de um tempo | A Steam verificou ou atualizou o jogo. Copie os arquivos de novo. |
| Interface **esticada** em ultrawide | Não é a tradução. É o jogo, e quem conserta é o **P5StrikersFix**, que não vem aqui e nunca veio. |
| Jogo **não abre** | Restaure os dois arquivos do backup e reporte o problema. |

---

## O que está traduzido

**Texto** — completo e revisado linha a linha: diálogos, menus, itens,
habilidades, descrições, solicitações, tutoriais e as legendas dos vídeos.

**Interface gráfica** — completa. No Persona 5 Strikers, boa parte da interface
**não é texto**: são imagens desenhadas, no estilo recortado da série. Trocar uma
palavra ali significa redesenhar o sprite, reproduzindo a fonte, o contorno, a
sombra e a inclinação do original.

A letra não é fonte instalada: ou é **colhida das outras sete variantes de idioma
da mesma textura** — cada letra recortada de onde o próprio jogo já a desenhou —
ou redesenhada com os maneirismos do estilo P5.

## O que ficou de fora, de propósito

- **Placas e cartazes do cenário** (farmácia, estação, lojas de rua). Ficam em
  japonês, como no jogo original — nem a localização oficial em espanhol as
  traduziu. Traduzir quebraria a ambientação de Tóquio.
- As **168 capturas de tutorial** e o **aviso legal em japonês da abertura**.

---

## Provavelmente o último patch

O jogo está traduzido por inteiro, texto e imagem, e a tradução está fechada
desde a v2.0. Não há mais frente aberta.

**Isso não significa abandono.** Bug reportado continua sendo corrigido — é
exatamente para isso que o projeto fica de pé. Se você encontrar qualquer coisa,
mande um print e o nome da tela.

### O que a versão anterior aguentou em uso real

- um jogador fechou as **47 de 47 conquistas em 75 horas** com a v2.0/v2.0.1;
- outro passou de **34 horas**;
- **nenhum bug de tradução reportado** em nenhum dos dois.

Platina exige concluir a história, todas as prisões, as solicitações e o conteúdo
pós-jogo — e várias conquistas dependem de cumprir objetivos cujo texto é nosso.
Um termo errado num objetivo teria travado o jogador.

---

## Créditos e avisos

- Tradução PT-BR: trabalho independente, sem vínculo com Atlus, SEGA ou
  Koei Tecmo.
- Agradecimento a **Ahtheerr** e **OTTYSS**.
- *Persona 5 Strikers* © ATLUS © SEGA / © KOEI TECMO GAMES. Todos os direitos
  reservados. Este é um projeto de fã, gratuito e sem fins lucrativos.
