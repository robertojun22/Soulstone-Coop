SOULSTONE COOP 1.6.0 - co-op para Soulstone Survivors: local (mesmo PC) e ONLINE (Steam), até 4 jogadores
=========================================================================================================

RECOMENDAÇÃO: JOGUE COM 2 JOGADORES
- Com 2 jogadores tudo está pronto, no local ou online: tela dividida, números de dano e miras nas cores de cada
  jogador.
- 3 e 4 jogadores funcionam, mas ainda estamos otimizando o desempenho: com muitos inimigos o jogo pode ficar
  pesado. Para 3 e 4 a câmera padrão é a "coleira" (uma tela só), a mais leve. O online com 3-4 jogadores de
  verdade ainda foi pouco testado.

REQUISITOS
- Windows, com Soulstone Survivors da Steam (testado na versão 1.5d2).
- BepInEx 6 (IL2CPP), build be.791. Ele já vem no pacote completo: não precisa baixar.
- Internet na PRIMEIRA abertura do jogo depois de instalar: o BepInEx baixa as bibliotecas do Unity e
  prepara os arquivos dele. A primeira abertura demora de 1 a 3 minutos com a tela parada. É normal.
- Co-op local: um controle por jogador extra. O teclado e o mouse contam como um jogador (só um teclado por PC).
- Online: todos os jogadores precisam do mod, na MESMA versão (1.6.0), e da Steam aberta.

QUAL ARQUIVO USAR
- SoulstoneCoop-1.6.0-full.zip: mod + o BepInEx certo. Use-o para instalar e para atualizar à mão: extraia por cima
  da pasta do jogo, substituindo tudo. As suas configurações são mantidas.
- SoulstoneCoop-1.6.0-mod-only.zip: só o mod, para gerenciadores de mods (formato Thunderstore, com manifest.json).
  Ele precisa do pacote do BepInEx "BepInExPack_IL2CPP 6.0.788" ou mais novo, que o gerenciador instala junto.

NÃO ATUALIZE O BEPINEX POR CONTA PRÓPRIA
- O Soulstone Survivors é um jogo IL2CPP e só funciona com o BepInEx 6 IL2CPP, a versão do pacote completo.
- A versão da página de releases do BepInEx no GitHub (5.4) é para jogos Unity "Mono" e NUNCA funciona neste
  jogo: instalada por cima do mod, o jogo abre sem carregar nenhum mod.
- Versões de teste mais novas do BepInEx 6 podem mudar coisas por dentro e quebrar o mod. Quando uma mais nova
  for segura, ela virá numa versão nova do mod.
- O mod sumiu depois de mexer no BepInEx? Extraia o pacote completo de novo por cima da pasta do jogo,
  substituindo tudo.

COMO INSTALAR (pacote completo)
1. Na Steam: clique com o botão direito em Soulstone Survivors > Gerenciar > Ver arquivos locais.
   Abre a pasta do jogo (onde está "Soulstone Survivors.exe").
2. Extraia TODO o conteúdo do zip DENTRO dessa pasta, mantendo as pastas.
   Ao final devem existir, ao lado do "Soulstone Survivors.exe":
     winhttp.dll
     doorstop_config.ini
     .doorstop_version
     dotnet\            (pasta)
     BepInEx\core\      (pasta)
     BepInEx\plugins\SoulstoneCoop.dll
3. Abra o jogo pela Steam normalmente e espere a primeira abertura terminar.

COMO JOGAR (local)
- No menu principal, entre no botão "Co-op".
- Cada jogador aperta A no próprio controle (ou Enter no teclado) para entrar. A ordem de entrada define P1, P2,
  P3 e P4. B ou Esc sai. O P1 confirma com START (ou Enter, se estiver no teclado).
- Cada jogador escolhe o próprio herói na vez dele. Na vez de um jogador extra, o botão "Lutar" vira "Pronto".
- Para refazer a entrada dos jogadores: na aba Lutar, aperte B no controle (ou Backspace no teclado) e confirme
  "Voltar ao menu inicial".
- Ajustes do co-op ficam em Opções > aba "Co-op" (LB/RB chegam até ela; cima/baixo escolhem, A marca a caixinha
  ou abre a lista, esquerda/direita mexem na barra). O (?) de cada linha explica a opção.

COMO JOGAR (online)
- Quem cria a partida (o host) abre a tela "Co-op" e aperta Y no controle (ou O no teclado) para criar a partida
  online; depois Y (ou O) de novo para convidar um amigo pela Steam. X (ou L) sai da sala.
- O amigo aceita o convite da Steam. Os dois escolhem os heróis; o Lutar espera todos ficarem prontos.
- Jogadores locais e online somam até 4 heróis no total (por exemplo: 2 num PC + 2 no outro).
- O host escolhe os mapas e os portais; o sigilo (Caça aos Titãs) e a dificuldade do host valem para todos.
- No meio da partida o host pode convidar de novo com F5 (quem caiu pode voltar com o mesmo herói).
- Se o host sair de uma partida de 2 jogadores, o outro vira o host e continua.
- Numa sala online ninguém libera heróis. O convidado fica com a experiência, as pedras da alma e os materiais que
  ganhar; mapas que o convidado ainda não liberou não são liberados jogando como convidado.
- Pular a animação de entrada de um chefe pula para todos.

CONFIGURAÇÃO AVANÇADA (opcional)
- Arquivo: BepInEx\config\SoulstoneCoop.cfg. Ele é criado na primeira abertura com os valores padrão.
- Quem atualiza de uma versão anterior NÃO precisa apagar esse arquivo: as opções novas entram sozinhas. Um valor
  que você tenha mudado à mão fica como está.
- Novo na 1.6.0: DirectSoulstones (ligado por padrão): as pedras da alma azuis vão direto para cada herói, sem os
  cristais voando (bem mais leve, mesma quantidade).

NOVIDADES DA 1.6.0
Co-op online (Steam)
- Jogue com amigos pela internet: crie uma sala, convide pela Steam, escolham os heróis e joguem juntos.
- Até 4 heróis no total, juntando jogadores locais e online.
- O host comanda a partida: inimigos, elites, Senhores, titãs e os ataques deles, altares e os objetivos deles,
  as orbes negras (fragmentos do vazio) da Caça aos Titãs, baús e a arena do chefe aparecem iguais em todos os PCs.
- O sigilo e a dificuldade do host valem para todos, então os inimigos têm a mesma vida e os mesmos bônus em
  todos os PCs.
- Todos veem as transformações e as invocações das habilidades únicas dos outros; os itens da habilidade única de
  cada jogador (cristais, fragmentos, pegadas...) só aparecem no PC do próprio jogador.
- O time divide uma barra de experiência; as subidas de nível se revezam entre os jogadores, e cada um escolhe as
  próprias cartas no próprio PC (a carta do titã também, uma para cada jogador).
- Pular a animação de entrada de um chefe pula para todos; todos são levados juntos para a arena do chefe.
- Quem cair da partida pode voltar no meio dela com o mesmo herói.

Desempenho
- Pedras da alma azuis creditadas direto em cada herói (sem milhares de cristais voando): grande ganho de FPS,
  principalmente para o convidado online.
- Menos operações pesadas por quadro no código do online.

Interface
- Todos os textos do mod (local e online) nos 13 idiomas do jogo, com a fonte do jogo.

PROBLEMAS CONHECIDOS
- Online: alguns minérios do mapa (os cristais que você quebra para ganhar materiais) podem não aparecer para o
  convidado.
- A barra da habilidade única do Caçador de Demônios na estátua pode piscar quando outro herói local fica na área
  da estátua junto com o Caçador.
- O online com 3 e 4 jogadores de verdade ainda foi pouco testado.
- Programas que criam controle virtual (Sunshine, Parsec, DS4Windows, Steam Input em alguns casos) podem fazer
  um controle físico aparecer duas vezes. Se um controle mexer dois heróis, feche o programa ou desative o
  controle virtual dele.
- 3 e 4 jogadores: com muitos inimigos o jogo pode ficar pesado, ainda mais com a tela dividida.
- Com 3-4 jogadores e câmeras em qualidade baixa, o círculo colorido embaixo de cada herói não aparece nas telas
  dos jogadores 2 a 4.
- Buffs que uma habilidade dá ao ACERTAR um inimigo não são compartilhados (só os que vêm ao lançar).

COMO DESINSTALAR
- Só o mod: apague BepInEx\plugins\SoulstoneCoop.dll.
- Tudo: apague winhttp.dll, doorstop_config.ini, .doorstop_version e as pastas BepInEx e dotnet da pasta do
  jogo. Outra opção é usar "Verificar integridade dos arquivos" na Steam depois de apagar winhttp.dll.

SEGURANÇA
- O co-op local não usa internet. O co-op online usa só a rede da própria Steam (salas da Steam e a conexão direta
  da Steam entre jogadores) enquanto você está numa sala online; o mod não abre portas por conta própria.
- O mod não edita saves: o jogo salva o seu progresso normalmente. O mod só grava o próprio arquivo de config e
  os logs.
- Baixe só de quem você confia: o BepInEx carrega qualquer DLL que estiver em BepInEx\plugins.

PARA RELATAR UM PROBLEMA
- Envie o arquivo BepInEx\LogOutput.log logo depois de fechar o jogo (ele recomeça a cada abertura) e diga o que
  aconteceu, quantos jogadores eram e se era local ou online (online: dos dois PCs, se der).

Créditos: BepInEx (https://github.com/BepInEx/BepInEx, licença LGPL-2.1), que traz o HarmonyX e o Il2CppInterop.
Licença do mod: CC BY-NC-SA 4.0 (https://creativecommons.org/licenses/by-nc-sa/4.0/).
Um pedido do autor: fique à vontade para compartilhar cópias deste mod em qualquer lugar, mas, por favor, não envie para o Nexus Mods.

CONFERÊNCIA (SHA256 do arquivo BepInEx\plugins\SoulstoneCoop.dll da versão 1.6.0):
DB1BB9332347D23122AC20B32B03782B3A708A82C22D4879EFC537C43B925683
No PowerShell: Get-FileHash "BepInEx\plugins\SoulstoneCoop.dll"
