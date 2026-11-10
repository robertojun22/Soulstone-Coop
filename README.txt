SOULSTONE COOP 1.6.0 - co-op for Soulstone Survivors: local (same PC) and ONLINE (Steam), up to 4 players
=========================================================================================================

RECOMMENDED: PLAY WITH 2 PLAYERS
- With 2 players everything is ready, local or online: split screen, damage numbers and crosshairs in each
  player's color.
- 3 and 4 players work, but we are still optimizing performance: with many enemies the game can get heavy. With
  3 and 4 the default camera is the "leash" (one shared screen), the lightest. Online with 3-4 real players has
  been tested very little so far.

REQUIREMENTS
- Windows, with Soulstone Survivors from Steam (tested on game version 1.5d2).
- BepInEx 6 (IL2CPP), build be.791. The full package already includes it: you don't need to download it.
- Internet on the FIRST game launch after installing: BepInEx downloads the Unity libraries and prepares its
  files. That first launch takes 1 to 3 minutes on a frozen screen. This is normal.
- Local co-op: one controller per extra player. Keyboard and mouse count as one player (only one keyboard per PC).
- Online: every player needs the mod, the SAME version (1.6.0), and Steam running.

WHICH FILE TO USE
- SoulstoneCoop-1.6.0-full.zip: mod + the right BepInEx. Use it to install and to update by hand: extract it over
  the game folder and overwrite everything. Your settings are kept.
- SoulstoneCoop-1.6.0-mod-only.zip: only the mod, for mod managers (Thunderstore format, with manifest.json). It
  needs the BepInEx pack "BepInExPack_IL2CPP 6.0.788" or newer, which the manager installs with it.

DO NOT UPDATE BEPINEX YOURSELF
- Soulstone Survivors is an IL2CPP game and only works with BepInEx 6 IL2CPP, the version in the full package.
- The version on the BepInEx GitHub releases page (5.4) is for Unity "Mono" games and NEVER works with this game:
  installed over the mod, the game starts without loading any mod.
- Newer BepInEx 6 test builds can change things inside and break the mod. When a newer one is safe, it will come
  in a new version of the mod.
- Mod gone after changing BepInEx? Extract the full package again over the game folder, overwriting everything.

HOW TO INSTALL (full package)
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
3. Start the game from Steam as usual and wait for the first launch to finish.

HOW TO PLAY (local)
- On the main menu, open the "Co-op" button.
- Each player presses A on their own controller (or Enter on the keyboard) to join. The join order sets P1, P2,
  P3 and P4. B or Esc leaves. P1 confirms with START (or Enter, if on the keyboard).
- Each player picks their own hero on their turn. On an extra player's turn, the start button becomes "Ready".
- To redo who joins: on the Fight tab, press B on a controller (or Backspace on the keyboard) and confirm
  "Back to the title screen".
- Co-op settings are in Options > "Co-op" tab (LB/RB reach it; up/down choose, A ticks the checkbox or opens the
  list, left/right move the slider). Each row's (?) explains it.

HOW TO PLAY (online)
- The host opens the "Co-op" screen and presses Y on the controller (or O on the keyboard) to create an online
  match, then Y (or O) again to invite a friend through Steam. X (or L) leaves the room.
- The friend accepts the Steam invite. Both pick their heroes; Fight waits until everyone is ready.
- Local and online players add up to 4 heroes in total (for example: 2 on one PC + 2 on another).
- The host picks the maps and the portals; the host's sigil (Titan Hunt) and difficulty apply to everyone.
- During a match the host can invite again with F5 (someone who dropped can come back with the same hero).
- If the host leaves a 2-player match, the other player becomes the host and goes on.
- In an online room nobody can unlock heroes. A guest keeps the experience, soulstones and materials earned;
  maps the guest hasn't unlocked yet are not unlocked by playing them as a guest.
- Skipping a boss's entrance animation skips it for everyone.

ADVANCED SETTINGS (optional)
- File: BepInEx\config\SoulstoneCoop.cfg. It is created on the first launch with the default values.
- If you are updating from an older version you do NOT need to delete this file: new options are added by
  themselves. A value you changed by hand is left as it is.
- New in 1.6.0: DirectSoulstones (on by default): the blue soulstones go straight to each hero, with no flying
  crystals (much lighter, same amount).

WHAT'S NEW IN 1.6.0
Online co-op (Steam)
- Play with friends over the internet: create a room, invite through Steam, pick heroes and play together.
- Up to 4 heroes in total, local and online players together.
- The host runs the match: enemies, elites, lords, titans and their attacks, altars and their objectives, the
  Titan Hunt's black orbs (void fragments), chests and the boss arena show the same on every PC.
- The host's sigil and difficulty are used by everyone, so enemies have the same life and bonuses on every PC.
- Everyone sees the other players' unique skill transformations and summons; each player's unique skill items
  (crystals, shards, tracks...) only appear on that player's own PC.
- The team shares one experience bar; the level-ups take turns between the players, and each player picks their
  own cards on their own PC (the titan card too, one for each player).
- Skipping a boss's entrance animation skips it for everyone; everyone is taken into the boss arena together.
- Someone who drops can come back during the match with the same hero.

Performance
- Blue soulstones credited straight to each hero (no thousands of flying crystals): a big FPS gain, above all for
  the online guest.
- Fewer heavy operations per frame in the online code.

Interface
- All the mod's texts (local and online) in the game's 13 languages, with the game's font.

KNOWN ISSUES
- Online: some of the map's mineral ores (the crystals you break for materials) may not appear for the guest.
- The Demon Hunter's unique skill bar on the statue can blink when another local hero stands in the statue's area
  with the Demon Hunter.
- Online with 3 and 4 real players has been tested very little.
- Programs that create a virtual controller (Sunshine, Parsec, DS4Windows, Steam Input in some cases) can make a
  physical controller show up twice. If one controller moves two heroes, close that program or turn off its
  virtual controller.
- 3 and 4 players: with many enemies the game can get heavy, more so with a split screen.
- With 3-4 players and low quality cameras, the colored circle under each hero doesn't show on players 2 to 4's
  screens.
- Buffs a skill gives when it HITS an enemy are not shared (only the ones given when it is cast).

HOW TO UNINSTALL
- Mod only: delete BepInEx\plugins\SoulstoneCoop.dll.
- Everything: delete winhttp.dll, doorstop_config.ini, .doorstop_version and the BepInEx and dotnet folders from
  the game folder. Another option is Steam's "Verify integrity of game files" after deleting winhttp.dll.

SAFETY
- Local co-op does not use the internet. Online co-op only uses Steam's own network (Steam rooms and Steam's
  peer-to-peer connection) while you are in an online room; the mod opens no ports by itself.
- The mod does not edit saves: the game saves your progress as usual. The mod only writes its own config file and
  logs.
- Only download from people you trust: BepInEx loads any DLL placed in BepInEx\plugins.

REPORTING A PROBLEM
- Send the file BepInEx\LogOutput.log right after closing the game (it starts over on every launch) and say what
  happened, how many players there were and whether it was local or online (online: from both PCs, if possible).

Credits: BepInEx (https://github.com/BepInEx/BepInEx, LGPL-2.1 license), which includes HarmonyX and Il2CppInterop.
Mod license: CC BY-NC-SA 4.0 (https://creativecommons.org/licenses/by-nc-sa/4.0/).
A request from the author: you are welcome to share copies of this mod anywhere, but please do not upload it to Nexus Mods.

CHECKSUM (SHA256 of BepInEx\plugins\SoulstoneCoop.dll for version 1.6.0):
DB1BB9332347D23122AC20B32B03782B3A708A82C22D4879EFC537C43B925683
In PowerShell: Get-FileHash "BepInEx\plugins\SoulstoneCoop.dll"
