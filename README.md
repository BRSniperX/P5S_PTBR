# Persona 5 Strikers — Tradução PT-BR (v1.1)

Tradução para português do Brasil de **Persona 5 Strikers** (PC / Steam).
Cobre o texto do jogo e boa parte da interface gráfica.

---

## Novidades da v1.1

- Refino técnico da tradução textual.

---

## ⚠️ REQUISITO OBRIGATÓRIO: o jogo tem que estar em ESPANHOL

Esta tradução **substitui os arquivos do idioma espanhol** do jogo. Ela não
adiciona um idioma novo — ela reescreve o espanhol em português.

**Jogar em outro idioma com a tradução instalada quebra o jogo.** Não é que o
português apenas deixa de aparecer: a interface fica corrompida, com textos
ilegíveis, embaralhados ou fora do lugar.

Por isso, deixar o jogo em espanhol **antes** de instalar não é uma
recomendação — é obrigatório.

### Como deixar o jogo em espanhol na Steam

1. Abra a **Biblioteca** da Steam.
2. Clique com o **botão direito** em *Persona 5 Strikers* → **Propriedades**.
3. Vá na aba **Idioma**.
4. Selecione **Espanhol**.
5. Espere a Steam baixar os arquivos do idioma (ela faz isso sozinha).
6. **Só então** instale esta tradução, seguindo os passos abaixo.

> Se você instalar a tradução antes de trocar o idioma, a Steam pode baixar os
> arquivos por cima e desfazer a instalação. Troque o idioma primeiro, sempre.

Versão pirata, de outra loja (Epic, GOG) ou de console **não** é suportada.
O projeto foi feito e testado na versão Steam para PC.

---

## Instalação

1. **Confirme que o jogo está em espanhol** (seção acima). Este é o passo que
   mais causa problema — não pule.
2. **Feche o jogo.**
3. Copie o conteúdo do .zip para a pasta onde o jogo está instalado, mantendo a
   estrutura. O caminho costuma ser:

   ```
   ...\steamapps\common\P5S\
   ```

   Ao final você deve ter:

   ```
   P5S\dinput8.dll
   P5S\update\HexPatcher.asi
   P5S\update\HexPatcher.ini
   P5S\update\data\motor_rsc\ScreenLayout.rdb
   P5S\update\data\motor_rsc\ScreenLayout.rdb.bin_9
   P5S\update\data\pd_ww\LINKDATA.BIN
   P5S\update\data\pd_ww\LINKDATA.IDX
   ```

4. Abra o jogo. O menu inicial deve aparecer em português, com o selo
   **PT-BR** embaixo do logo do P5S.

### Não funcionou? Comece por aqui

| O que você vê | Causa quase certa |
|---|---|
| Textos **embaralhados** ou ilegíveis | O idioma na Steam não está em espanhol. Troque para espanhol e reinstale. |
| Jogo em **espanhol**, sem nada em português | Os arquivos não foram para a pasta certa. Confira a lista acima, caminho por caminho. |
| Português sumiu depois de um tempo | A Steam verificou/atualizou os arquivos. Reinstale a tradução. |
| Jogo não abre | Restaure sua cópia da pasta `update\` e reporte o problema. |

### Antes de instalar, faça backup

Este pacote **não** substitui arquivos originais do jogo — tudo vai para a
pasta `update\`, que tem prioridade sobre os dados originais. Ainda assim,
guarde uma cópia de `update\` se você já tiver outros mods ali.

### Para desinstalar

Apague os arquivos listados acima. Se a pasta `update\` já era sua e tinha
outras coisas, apague apenas os arquivos desta lista.

---

## O que está traduzido

**Texto** — completo: diálogos, menus, itens, habilidades, descrições,
solicitações e tutoriais.

**Interface gráfica** — esta é a parte trabalhosa. No Persona 5 Strikers, boa
parte da interface **não é texto**: são imagens desenhadas, no estilo recortado
da série. Trocar uma palavra ali significa redesenhar o sprite, reproduzindo a
fonte, o contorno, a sombra e a inclinação do original. Foi feito assim, área
por área:

### Menus

Tudo que se acessa pelo botão de menu:

- **Menu inicial**: `NOVO JOGO`, `CARREGAR JOGO`, `CONFIG.`, `SAIR`, e o
  "aperte qualquer botão"
- **Menu de pausa**: `TUTORIAL`, `CARREGAR DADOS`, `SALVAR DADOS`,
  `VOLTAR À TELA DE TÍTULO`, `SAIR DO JOGO`
- **Abas e telas internas**: itens, equipamento, status, vínculos e registro
- **Configurações**: dificuldade, vibração, legendas, exibir dano, guia de
  controles, inverter câmera e as opções de vídeo
- **Os 24 Arcanos** (Louco, Mago, Sacerdotisa, Imperatriz…)
- **Sala de Veludo**: `Criar Novas Personas`, `Melhoria de Persona`,
  `Registrar/Invocar Personas`, com as legendas de cada opção

### HUD de batalha

O que aparece na tela durante o combate:

- Reações de acerto: `FRACO`, `BLOQUEIO`, `MUNIÇÃO`
- Rastreador de missão: `MISSÃO`, `NOVA`, e o banner grande de objetivo
- Resultado: `MANDOU BEM`, `MISSÃO CUMPRIDA`, `ITEM OBTIDO`, `DINHEIRO`,
  `EXP DE VÍNCULO`
- Abreviações de elemento e os ícones de categoria de habilidade

### HUD de exploração

O que aparece andando pelas prisões e pela cidade:

- **Ações contextuais** — os comandos que surgem perto de objetos e pessoas:
  `Atacar!`, `Examinar!`, `Mexa-se!`, `Falar`, `Loja` e outros
- **Placa de setas das prisões**, com os destinos, mais a tela de seleção de
  equipe
- **Atalhos do HUD** — os 62 rótulos de comando que aparecem no rodapé
- **Caixa de diálogo**: `Avançar`, `Pular`, `Auto ATIVADO/DESATIVADO`

### Calendário e data

- Os **dias da semana** e a **data** exibidos no canto da tela
- A **tela de transição de dia**, com as três camadas sobrepostas do desenho
  original preservadas

## O que NÃO está traduzido

Sendo honesto sobre os limites desta versão:

- **Placas e cartazes do cenário** (farmácia, estação, lojas de rua). Ficam em
  japonês, como no jogo original — nem a localização oficial em espanhol as
  traduziu. Traduzir quebraria a ambientação de Tóquio.
- **Parte das imagens de interface**, que ainda aparecem em espanhol. Como a
  tradução parte do espanhol, o que ainda não foi redesenhado continua no
  idioma de origem.

---

## Créditos e avisos

- Tradução PT-BR: trabalho independente, sem vínculo com Atlus, SEGA ou
  Koei Tecmo.
- Agradecimento a **OTTYSS**.
- `dinput8.dll` e `HexPatcher.asi` são componentes de terceiros, incluídos
  apenas para facilitar a instalação. Os créditos e a licença pertencem aos
  seus autores.
- *Persona 5 Strikers* © ATLUS © SEGA / © KOEI TECMO GAMES. Todos os direitos
  reservados. Este é um projeto de fã, gratuito e sem fins lucrativos.

## Problemas conhecidos

Ainda há artes da interface em espanhol, que serão corrigidas em versões
futuras.

Encontrou algo além disso? Reporte com um print e o nome da tela.
