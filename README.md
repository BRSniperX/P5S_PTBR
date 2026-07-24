# Persona 5 Strikers — Tradução PT-BR v1.2

Tradução para português do Brasil de **Persona 5 Strikers** (PC / Steam).
Cobre o texto do jogo e boa parte da interface gráfica.

> ⚠️ **O jogo precisa estar em ESPANHOL.** Esta tradução reescreve os arquivos
> do idioma espanhol — ela não adiciona um idioma novo. Jogar em outro idioma
> com ela instalada deixa a interface corrompida.

---

## Novidades da v1.2

**Menu do esconderijo** — as placas do acampamento agora estão em português:
`FALAR`, `COZINHAR`, `USAR LOJA`, `VER SOLICITAÇÕES`, `ENVIAR AVISO`,
`INFILTRAR NA PRISÃO`, `ENTRAR NA SALA DE VELUDO`, `IR AO DESTINO`,
`IR À PRÓXIMA CIDADE` e `SAIR`.

**Loja da Sophia** — a tela inteira: `Preço`, `Em posse`, `Dinheiro`,
`Inventário`, `Informação`, os cabeçalhos de compra e venda, `Esgotado`,
`Novo`, `Ienes` e as confirmações.

**Cozinha e investigação** — `O que eu cozinho?`, `Necessário`, `Dá pra fazer`,
`INVESTIGAÇÃO`, `COMEÇAR`, `ESCREVA SEU NOME` e o `ACEITAR`. Três desses
rótulos ainda estavam em **japonês** na versão espanhola do jogo.

**Data no esconderijo** — dias da semana e períodos do dia, que ali continuavam
em espanhol mesmo com o HUD já traduzido.

**Sala de Veludo** — o `Nueva entrada` da tela de registro virou `Nova entrada`.

**Configurações** — o `DESACTIVADO`/`ACTIVADO` inclinado que aparece na opção
não selecionada.

### Correções de texto

- Ryuji falava de si no feminino numa fala do beco de Shibuya.
- Uma fala da Ann em Shibuya vazava para fora do balão.
- A descrição do curativo partia o número "20" no meio, na quebra de linha.

---

## Instalação

1. Deixe o jogo em **espanhol** pela Steam
   (*Propriedades* → *Idioma* → *Espanhol*) e espere o download terminar.
2. **Feche o jogo.**
3. Extraia o conteúdo do `.zip` na pasta do jogo, mantendo a estrutura —
   normalmente `...\steamapps\common\P5S\`.

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

Abra o jogo: o menu inicial deve aparecer em português, com o selo **PT-BR**
embaixo do logo.

**Já tem a v1.0 ou a v1.1?** É só substituir os arquivos por cima.

### Não funcionou?

| O que você vê | Causa quase certa |
|---|---|
| Textos embaralhados ou ilegíveis | O idioma na Steam não está em espanhol |
| Jogo em espanhol, sem nada em português | Os arquivos não foram para a pasta certa |
| O português sumiu depois de um tempo | A Steam verificou os arquivos; reinstale |
| O jogo não abre | Restaure sua cópia de `update\` e reporte |

Nada aqui substitui arquivo original do jogo — tudo vai para a pasta `update\`,
que tem prioridade sobre os dados originais. Para desinstalar, apague os
arquivos da lista acima.

---

## Problemas conhecidos

Ainda restam artes da interface em espanhol. A conhecida que falta é o rótulo
vermelho `ABIERTO`, dos espaços de habilidade vazios: o sprite ainda não foi
localizado nos arquivos do jogo.

As **placas e cartazes do cenário** (farmácia, estação, lojas de rua) ficam em
japonês de propósito — nem a localização oficial em espanhol as traduziu, e
traduzir quebraria a ambientação de Tóquio.

Encontrou algo além disso? Abra uma issue com um print e o nome da tela.

---

Agradecimento a **OTTYSS**.

`dinput8.dll` e `HexPatcher.asi` são componentes de terceiros, incluídos apenas
para facilitar a instalação; os créditos e a licença pertencem aos seus autores.

*Persona 5 Strikers* © ATLUS © SEGA / © KOEI TECMO GAMES. Todos os direitos
reservados. Projeto de fã, gratuito e sem fins lucrativos, sem vínculo com
Atlus, SEGA ou Koei Tecmo.
