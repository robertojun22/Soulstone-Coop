# Soulstone Coop

*English below   /   Português abaixo*

## 🇺🇸 English

### What it is
Soulstone Coop turns Soulstone Survivors into a **local** co-op game: 2 to 4 people on the same PC, each with their own
hero, their own health and skill bar, and their own controller. No internet needed, and your saves are not touched.

### How to start a co-op match
1. In the main menu, open **Co-op**.
2. Each player presses **A** on their own controller (or **Enter** on the keyboard) to join. The joining order sets
   P1, P2, P3 and P4. **B**/**Esc** leaves. Keyboard and mouse count as one player (one keyboard per PC).
3. **P1** confirms with **START** (or **Enter** if on the keyboard).
4. On the hero screen, each player picks on their turn (extras first, P1 last). On an extra's turn the "Fight"
   button becomes "Ready". Each hero can only be picked once.
5. P1 picks the map and presses **Fight**. Everyone spawns together with their own hero, weapon, skin and runes.

To redo who joins, press **B** (controller) or **Backspace** on the Fight tab and confirm "Back to the title screen".

### How it works
- **Separate controls:** every player moves, aims and dashes with their own controller. Manual aim works with the
  right stick or the mouse. Each player has their own auto-aim, and rumble only goes to the controller of the
  player who was hit.
- **Shared camera ("Leash"):** the camera frames the whole group and zooms out as you spread apart. At the maximum
  zoom nobody can walk off screen.
- **XP and levels:** XP is shared and everyone collects it. On each level-up, every player picks a card on their
  turn. The cards are tinted in that player's color with their P1–P4 badge. Only the picking player's controller
  works. On a keyboard player's turn, the prompts show keyboard keys.
- **Game options for everyone:** each player has their own "skip active skills" checkbox and can replace a skill
  when their bar is full. The levels that offer new skills rotate between players.
- **Per-player HUD:** each player has a health and skill bar in their color, with their Pn badge. Each bar has as
  many slots as that hero can hold, including the extra rune slot. Each hero also has a health bar over the head in
  the player's color (always visible, with their dash charges), a colored ring on the ground, an optional P1–P4 tag,
  a minimap icon and a colored crosshair.
- **Death and revive:** Death Protections (extra lives) are shared. A downed player sits in a revive zone, and an
  ally standing in it brings them back with 50% health and 1 second of invulnerability. The body stays put while
  down. The match only ends when everyone is down. Surrendering ends the match for everyone.
- **Difficulty:**
  - Enemies: 2.5x with 2 players, 3.5x with 3 and 4.25x with 4, split between the players.
  - Elites and final bosses: 1.17x / 1.33x / 1.5x health. Void Lords: 1.33x / 1.67x / 2x health.
  - Each wave of Void Lords gets +1 lord per extra player (at most +2), split between you, never the same lord
    twice in a wave.
  - The objective counters ("Eliminate the Void Lords", "monsters to summon a Lord") grow by the same ratio.
- **Titan power cards** go to every player (each gets their own copy).
- **Smart enemy pace:** an automatic controller keeps the map near a target number of living enemies. It spawns
  more when there are few and fewer when there are many. It also eases off a little when the team's health is low:
  below 70% health the target drops, down to 60% of the target when the team is at 30% or less.
- **Shared:**
  - Health crystals heal everyone, each player with their own healing bonuses.
  - While everyone is on screen, buffs a skill gives when it is cast apply to the whole group. Buffs from unique
    skills are not shared.
- **Unique-skill pickups** (souls, Abomination parts, Elementalist orbs, pirate treasure, etc.) can only be collected
  by the hero they belong to.
- **Stage changes:** when you go through a portal (endless mode, next stage), every player keeps what they had picked.

### Options menu (Options > "Co-op" tab)
Use LB/RB to reach the tab. Use the D-pad or stick to choose and A to confirm.
- **P1..P4 tags over the heroes:** Show / Hide.
- **Shared buffs:** On / Off.
- **Enemies on screen:** 50% to 100% of the game's target, in 5% steps (default 90%).

The camera is shared, with the leash; split screen will come in a future version.
More settings are in `BepInEx\config\SoulstoneCoop.cfg`. A [Testing] section left from old versions does nothing.

### Requirements
- Windows and Soulstone Survivors on Steam (tested on version 1.5d2).
- BepInEx 6 IL2CPP (be.788). It is already in the "completo" (full) package.
- Internet on the first launch after installing (BepInEx downloads Unity libraries).
- One controller per extra player (or keyboard and mouse for one of them).

### Installation
1. Steam > right-click Soulstone Survivors > Manage > **Browse local files**.
2. Extract **everything** from the zip into that folder, next to `Soulstone Survivors.exe`, keeping the folders:
   - `SoulstoneCoop-1.3.0-completo.zip`: if you don't have BepInEx yet (most people).
   - `SoulstoneCoop-1.3.0-so-o-mod.zip`: if you already have BepInEx 6 IL2CPP (or an older version of the mod). It only
     adds `BepInEx\plugins\SoulstoneCoop.dll`.
3. Start the game from Steam. The first launch takes 1–3 minutes on a still screen, which is normal.

### Uninstall
- **Mod only:** delete `BepInEx\plugins\SoulstoneCoop.dll`.
- **Everything:** delete `winhttp.dll`, `doorstop_config.ini`, `.doorstop_version` and the `BepInEx` and `dotnet`
  folders from the game folder. You can then run "Verify integrity of game files" in Steam.

### Known issues
- **Virtual controllers (Sunshine, Parsec, DS4Windows, sometimes Steam Input):** one physical controller may show up
  twice. The Co-op screen lets one controller join at a time. If one controller moves two heroes, close that program
  or turn off its virtual controller.
- **Split screen:** not available yet.
- Buffs a skill gives **when it hits** an enemy are not shared yet (only the ones given when it is cast).
- Steam achievements may be easier to get in co-op.

## 🇧🇷 Português

### O que é
Soulstone Coop transforma Soulstone Survivors num jogo cooperativo **local**: de 2 a 4 pessoas no mesmo PC, cada uma
com o seu herói, a sua barra de vida e habilidades e o seu controle. Não precisa de internet e não mexe nos seus saves.

### Como criar uma partida em co-op
1. No menu principal, entre em **Co-op**.
2. Cada jogador aperta **A** no próprio controle (ou **Enter** no teclado) para entrar. A ordem de entrada define
   P1, P2, P3 e P4. **B**/**Esc** sai. Teclado e mouse contam como um jogador (um teclado por PC).
3. O **P1** confirma com **START** (ou **Enter**, se estiver no teclado).
4. Na tela de heróis, cada um escolhe na sua vez (os extras primeiro, o P1 por último). Na vez de um extra, o
   botão "Lutar" vira "Pronto". Cada herói só pode ser escolhido uma vez.
5. O P1 escolhe o mapa e aperta **Lutar**. Todos entram juntos, cada um com o seu herói, arma, skin e runas.

Para refazer a entrada dos jogadores, aperte **B** (controle) ou **Backspace** na aba Lutar e confirme "Voltar ao menu
inicial".

### Como funciona
- **Controles separados:** cada jogador anda, mira e usa dash com o próprio controle. A mira manual funciona pelo
  analógico direito ou pelo mouse. A mira automática é de cada um, e a vibração vai só para o controle de quem tomou
  o golpe.
- **Câmera compartilhada ("Coleira"):** a câmera enquadra todo o grupo e afasta o zoom conforme vocês se espalham.
  No zoom máximo, ninguém consegue sair da tela.
- **Experiência e níveis:** a experiência é compartilhada e todos coletam. A cada subida de nível, cada jogador
  escolhe uma carta na sua vez. As cartas ficam na cor do jogador, com o selo P1–P4. Só o controle de quem está
  escolhendo funciona. Na vez de quem joga no teclado, a tela mostra as teclas do teclado.
- **Opções do jogo para todos:** cada jogador tem a sua caixinha "pular habilidades ativas" e pode substituir
  uma habilidade quando a barra está cheia. Os níveis que oferecem habilidades se revezam entre os jogadores.
- **HUD por jogador:** cada jogador tem uma barra de vida e de habilidades na sua cor, com o selo Pn. O número de
  espaços de cada barra segue o herói, incluindo o espaço extra de runa. Cada herói tem também uma barra de vida
  sobre a cabeça na cor do jogador (sempre visível, com as cargas de dash), um anel colorido no chão, a etiqueta
  P1–P4 (opcional), um ícone no minimapa e uma mira colorida.
- **Morte e revive:** as Proteções Contra Morte (vidas extras) são compartilhadas. Quem cai fica numa zona de
  revive, e um aliado parado nela o levanta com 50% de vida e 1 segundo de invulnerabilidade. O corpo fica parado
  enquanto o jogador está caído. A partida só acaba quando todos caem. Desistir encerra a partida para todos.
- **Dificuldade:**
  - Inimigos: 2,5x com 2 jogadores, 3,5x com 3 e 4,25x com 4, divididos entre os jogadores.
  - Elites e chefes finais: 1,17x / 1,33x / 1,5x de vida. Senhores do Vazio: 1,33x / 1,67x / 2x.
  - Cada leva de Senhores ganha +1 Senhor por jogador extra (no máximo +2), divididos entre vocês, sem repetir o
    mesmo Senhor na leva.
  - Os contadores de objetivo ("Elimine os Senhores", "monstros para conjurar um Senhor") crescem na mesma
    proporção.
- **Cartas de poder dos titãs** vão para todos os jogadores (cada um recebe a própria cópia).
- **Ritmo de inimigos inteligente:** um controle automático mantém o mapa perto de uma meta de inimigos vivos.
  Gera mais quando há poucos inimigos e menos quando há muitos. Também alivia um pouco quando a vida da equipe está
  baixa: abaixo de 70% de vida a meta diminui, até 60% da meta com a equipe em 30% ou menos.
- **Compartilhado:**
  - Cristais de cura curam todos, e cada um recebe os próprios bônus de cura.
  - Com todos na tela, os buffs que uma habilidade dá ao ser lançada valem para o grupo. Buffs de habilidades
    únicas não entram.
- **Itens de habilidade única** (almas, peças da Abominação, esferas da Elementalista, tesouro pirata etc.) só podem
  ser coletados pelo herói dono.
- **Troca de fase:** ao entrar num portal (modo infinito, próxima fase), todos os jogadores mantêm o que já tinham
  escolhido.

### Menu de opções (Opções > aba "Co-op")
Use LB/RB para chegar na aba. Use as setas ou o analógico para escolher e A para confirmar.
- **Etiquetas P1..P4 sobre os heróis:** Mostrar / Esconder.
- **Buffs compartilhados:** Ligado / Desligado.
- **Inimigos na tela:** de 50% a 100% do alvo do jogo, em passos de 5% (padrão 90%).

A câmera é compartilhada, com coleira; a tela dividida virá numa versão futura.
Mais ajustes ficam em `BepInEx\config\SoulstoneCoop.cfg`. A seção [Testing] que sobrou de versões antigas não faz nada.

### Requisitos
- Windows e Soulstone Survivors da Steam (testado na versão 1.5d2).
- BepInEx 6 IL2CPP (be.788). Já vem no pacote "completo".
- Internet na primeira abertura depois de instalar (o BepInEx baixa as bibliotecas do Unity).
- Um controle por jogador extra (ou teclado e mouse para um deles).

### Instalação
1. Steam > botão direito em Soulstone Survivors > Gerenciar > **Ver arquivos locais**.
2. Extraia **todo** o conteúdo do zip dentro dessa pasta, ao lado de `Soulstone Survivors.exe`, mantendo as pastas:
   - `SoulstoneCoop-1.3.0-completo.zip`: para quem ainda não tem BepInEx (o mais comum).
   - `SoulstoneCoop-1.3.0-so-o-mod.zip`: para quem já tem o BepInEx 6 IL2CPP (ou uma versão anterior do mod). Coloca
     só `BepInEx\plugins\SoulstoneCoop.dll`.
3. Abra o jogo pela Steam. A primeira abertura demora de 1 a 3 minutos com a tela parada, e isso é normal.

### Desinstalação
- **Só o mod:** apague `BepInEx\plugins\SoulstoneCoop.dll`.
- **Tudo:** apague `winhttp.dll`, `doorstop_config.ini`, `.doorstop_version` e as pastas `BepInEx` e `dotnet` da
  pasta do jogo. Se quiser, depois use "Verificar integridade dos arquivos" na Steam.

### Problemas conhecidos
- **Controle virtual (Sunshine, Parsec, DS4Windows, às vezes Steam Input):** um controle físico pode aparecer duas
  vezes. A tela Co-op aceita um controle por vez. Se um controle mexer dois heróis, feche o programa ou desative o
  controle virtual dele.
- **Tela dividida:** ainda não disponível.
- Buffs que uma habilidade dá **ao acertar** um inimigo ainda não são compartilhados (só os que vêm ao lançar).
- As conquistas da Steam podem ficar mais fáceis em co-op.
