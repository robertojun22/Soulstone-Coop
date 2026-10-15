SOULSTONE COOP 1.3.0 - local co-op for Soulstone Survivors (2 to 4 players on the same PC)
=========================================================================================

REQUIREMENTS
- Windows, with Soulstone Survivors from Steam (tested on game version 1.5d2).
- BepInEx 6 (IL2CPP), build be.788. The "completo" (full) package already includes BepInEx.
- Internet on the FIRST game launch after installing: BepInEx downloads the Unity libraries and prepares its
  files. That first launch takes 1 to 3 minutes on a frozen screen. This is normal.
- One controller per extra player. Keyboard and mouse count as one player (only one keyboard per PC).

WHICH FILE TO USE
- SoulstoneCoop-1.3.0-completo.zip -> full package, for anyone who does NOT have BepInEx in the game yet (most people).
- SoulstoneCoop-1.3.0-so-o-mod.zip -> mod only, for anyone who ALREADY has BepInEx 6 IL2CPP in Soulstone Survivors
  (if you already use an older version of the mod, this one just replaces the DLL).

HOW TO INSTALL
1. In Steam: right-click Soulstone Survivors > Manage > Browse local files.
   This opens the game folder (where "Soulstone Survivors.exe" is).
2. Extract ALL the contents of the zip INTO that folder, keeping the folders.
   When done, these must exist next to "Soulstone Survivors.exe":
     winhttp.dll
     doorstop_config.ini
     .doorstop_version
     dotnet\            (folder)
     BepInEx\core\      (folder)
     BepInEx\plugins\SoulstoneCoop.dll
   (The "mod only" package contains just BepInEx\plugins\SoulstoneCoop.dll.)
3. Start the game from Steam as usual and wait for the first launch to finish.

HOW TO PLAY
- On the main menu, open the "Co-op" button.
- Each player presses A on their own controller (or Enter on the keyboard) to join. The join order sets P1, P2,
  P3 and P4. B or Esc leaves. P1 confirms with START (or Enter, if on the keyboard).
- Each player picks their own hero on their turn. On an extra player's turn, the start button becomes "Ready".
- To redo who joins: on the Fight tab, press B on a controller (or Backspace on the keyboard) and confirm
  "Back to the title screen".
- Co-op settings are in Options > "Co-op" tab (LB/RB reach it; arrows and A change the options): P1..P4 tags over
  the heroes, shared buffs and how many enemies are on screen.

ADVANCED SETTINGS (optional)
- File: BepInEx\config\SoulstoneCoop.cfg. It is created on the first launch with the default values.
- If you are updating from an older version you do NOT need to delete this file: new options are added by
  themselves, and the old elite toughness value (0.5) is moved to the new default automatically. A value you
  changed by hand is left as it is. The leftover [Testing] section from old versions does nothing.
- New options in 1.3.0: [Coop] ShareTitanCards (titan cards for everyone), MaxExtraLords (extra lords per wave),
  LordToughnessPerExtraPlayer (lord health), RegularToughnessPerPlayerAbove2 (regular enemy health with 3 or 4
  players; default 0), SkillSlotsLessPerPlayerAbove2 (fewer skill slots with 3 or 4 players; default 0 = off);
  [HUD] OwnPendingLevelUps and BackToTitleButton.

WHAT'S NEW IN 1.3.0
Balance
- Regular enemies and elites: 2.5x with 2 players, 3.5x with 3 and 4.25x with 4 (before: 2.5x, 4x and 5.5x). The
  3rd and 4th players add fewer enemies, and the game runs lighter with 4 players.
- Elites and final bosses (titans and the campaign's final bosses): 1.17x health with 2 players, 1.33x with 3 and
  1.5x with 4.
- Void Lords: +1 per player beyond the first, at most +2 per wave; health 1.33x with 2 players, 1.67x with 3 and
  2x with 4. A wave never repeats the same lord (before, once the game's list ran out, the last one kept coming:
  up to 6 Medusas), and Medusa and Plaguebringer never come together.
- "Eliminate monsters to summon a Lord": the total grows with the number of enemies, rounded to the hundred
  (400 becomes 1000 with 2 players, 1400 with 3 and 1700 with 4).
- The wave pace speeds up at most 2x (before 3x).
- Chest and crystal guardians and the loot enemy are no longer multiplied.
- Titan power cards go to everyone: each player gets their own copy (skill cards stay with whoever picked them).
- Unique-skill items: when a hero already has 30 on the map, a new item replaces the one farthest from them
  (before, items stopped dropping).

Fixes
- Enemy bodies now really disappear faster with more players (in 1.2.0 this option had no effect).
- Unique skills work again when a hero gets back up. Before, a hero's death could stop their unique skill until the
  end of the match (and P1's death stopped everyone's): their items stopped dropping.
- Unique skills of players 2 to 4 (Sentinel's panther, Demon Hunter and others) are set up again automatically when
  they fail while the hero is created.
- Enemies near an extra player no longer vanish for being far from P1.
- A downed player's body stays put on the ground: allies and enemies no longer push it around. If the fall throws
  it far away, it comes back to where the player fell.
- Level-up screen: each player gets the number of card options from their own runes (before, P1's runes counted for
  everyone, and a P1 rune with fewer options left everyone with 2 cards).
- An extra player with more skill slots than P1 can replace their last skill when the bar is full.
- "Survive" map task: the mod mistook it for the Titan Hunt's Void presence event (it enlarged its barrier by
  mistake and read the wrong data).
- Less work for the mod on the title screen and the hub.

Interface
- Bottom health and skill bars in each player's color. The unique-skill panels are centered over each player's
  health bar, and the extra lives icon sits a little higher.
- A health bar over each hero's head, in the player's color and always visible, with the dash charges next to it
  (a hero who can't dash, like the Death Knight on his horse, shows no charges).
- Own pending level-ups counter, at the left of the level bar.
- P1's auto-aim icon is hidden in co-op (it sat on top of another player's bar).
- The colored ring on the ground follows the terrain and hides when the hero goes down.
- Co-op tab: new "P1..P4 tags over the heroes" option (Show / Hide). The camera choice left the tab until split
  screen is ready (the camera stays shared, with the leash).
- On the Fight tab, B on a controller or Backspace on the keyboard goes back to the title screen (with a
  confirmation), to redo who joins.
- The Co-op button shows up right on the very first title screen (before, hovering the first button lit up Co-op).
- The game window comes to the front on launch (the BepInEx console used to steal the focus).

WHAT'S NEW IN 1.2.0
- Unique-skill items dropped by killed enemies: the chance is divided by the number of players and each hero has
  at most 30 on the map.
- Menu: no longer freezes for a few seconds when leaving the hero screen while the model is still loading.
- Co-op tab: no longer changes options by itself while the settings are closed.
- Fewer stutters in long matches.
- Lords: the "kill X monsters to summon" counter no longer goes negative.
- Sentinel's panther also appears when the Sentinel is not P1.
- Extra lives of players 2 to 4 are used like P1's (original effect, voice and slow motion).

KNOWN ISSUES
- Programs that create a virtual controller (Sunshine, Parsec, DS4Windows, Steam Input in some cases) can make a
  physical controller show up twice. The Co-op screen accepts one controller at a time. If one controller moves two
  heroes, close that program or turn off its virtual controller.
- Split screen is not available yet. The camera is shared, with a "leash".
- Buffs a skill gives when it HITS an enemy are not shared (only the ones given when it is cast).

HOW TO UNINSTALL
- Mod only: delete BepInEx\plugins\SoulstoneCoop.dll.
- Everything: delete winhttp.dll, doorstop_config.ini, .doorstop_version and the BepInEx and dotnet folders from
  the game folder. Another option is Steam's "Verify integrity of game files" after deleting winhttp.dll.

SAFETY
- The mod does not use the internet, opens no ports and does not touch saves. It only reads and writes its own
  config file and the BepInEx log.
- Only download from people you trust: BepInEx loads any DLL placed in BepInEx\plugins.

REPORTING A PROBLEM
- Send the file BepInEx\LogOutput.log right after closing the game (it starts over on every launch) and say what
  happened and how many players there were.

Credits: BepInEx (https://github.com/BepInEx/BepInEx, LGPL-2.1 license), which includes HarmonyX and Il2CppInterop.
Mod license: CC BY-NC-SA 4.0 (https://creativecommons.org/licenses/by-nc-sa/4.0/).

CHECKSUM (SHA256 of BepInEx\plugins\SoulstoneCoop.dll for version 1.3.0):
9517E00E650FB6C4B75B1387865B9F72B9BF443622CA089731E42B2502ADD26D
In PowerShell: Get-FileHash "BepInEx\plugins\SoulstoneCoop.dll"
