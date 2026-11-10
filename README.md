# Veil Client

A Minecraft **1.8.9 PvP client** (Forge mod) made for **Bedwars** and **Skywars**, by Teri.

**NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.**

Fair-play only: no cheats, nothing that gives an unfair advantage, and the client never sends anything to the
server on its own. Everything it adds is visual or happens on your screen.

## Easiest way: use the Veil Client launcher

The [Veil Client launcher](https://github.com/TheDarkTeri/Veil-Client-Launcher-Releases) installs Java 8, Minecraft
1.8.9, Forge and Veil for you and keeps Veil updated: install it, sign in with Microsoft and press **Play**. Needs
Windows 10 or 11, 64-bit.

**[Download the launcher](https://github.com/TheDarkTeri/Veil-Client-Launcher-Releases/releases/latest)**

## Installing the mod yourself

Prefer your own launcher? **[Download the latest mod jar](https://github.com/TheDarkTeri/Veil-Client-Releases/releases/latest)**,
then:

1. Install **Forge 1.8.9** (11.15.1.2318 recommended) and launch it once.
2. Download `veil_client-<version>.jar` from [Releases](https://github.com/TheDarkTeri/Veil-Client-Releases/releases).
3. Put the jar in your `.minecraft/mods` folder (or your launcher instance's `mods` folder).
4. Start the game and press **Right Shift** to open the Veil menu.

Minecraft 1.8.9 runs on **Java 8**. OptiFine (1.8.9 HD U M5) works alongside Veil.

### Updating

Delete the old `veil_client-<old version>.jar` from your `mods` folder, then add the new one. Two Veil jars at
once will stop the game from starting. Your settings are kept.

### Only download Veil from here

The only official downloads are on this page's [Releases](https://github.com/TheDarkTeri/Veil-Client-Releases/releases).
A Veil jar from anywhere else may be modified and could steal your account.

## Using it

- **Right Shift** opens the mod menu. Left-click a module to turn it on or off, right-click it for its settings
  (including a key to toggle it in game).
- **Edit HUD** lets you drag, snap and resize everything on your screen.
- **Profiles** keep separate setups, for example one for Bedwars and one for Skywars.
- **Social** (in the Esc menu and on the main menu, or a key you set in Controls) has your Veil friends and
  messages.

## Features

- **HUD:** FPS, CPS, Coordinates, Keystrokes, Armor Status, Low Durability warning, Saturation, Hotbar Tweaks,
  Potion Status, Item Counter, Compass, Combo, Reach, Speed, Memory, Pack Display, Ping, Server Address, Clock,
  Session Stats (kills, finals, beds and wins), Generator Timers (Bedwars), Scoreboard, Boss Bar, Titles,
  Tab Ping, Bedwars Stats (see below), Screenshot Helper
- **Player:** Toggle Sprint, Nick Hider, Own Nametag (F5), Cape (other Veil players see it too), Friends (status,
  messages and invites; see below), Requeue key, Quick Play menu (Hypixel), Discord Presence (Windows)
- **Chat:** Name Mentions, Timestamps, Compact Chat, Chat Tweaks, Chat Tabs (All, Party, Guild, PMs), Auto GG
- **World:** Fullbright, Time Changer, Weather Changer, Waypoints
- **Render:** Zoom, Custom Crosshair, 1.7 Animations, Block Outline, Hit Color, Hitboxes, Item Physics,
  Enchant Glint, No Hurt Cam, Motion Blur, Particles, Menu Blur, Menu Music, Performance
- A custom red-and-black main menu, pause menu and menu backgrounds

### Bedwars Stats and your Hypixel API key

Bedwars Stats shows stars, FKDR and WLR next to names in the tab list on Hypixel. It needs **your own** API key
from [developer.hypixel.net](https://developer.hypixel.net), which requires a Minecraft account linked to Hypixel.

**Use it at your own risk.** Hypixel's rules say development keys are meant for your own projects, so Hypixel may
revoke a key used in a mod like this. Only your key is affected, not your Minecraft or Hypixel account. Never share
your key with anyone, and nobody from Veil will ever ask for it.

### Online features and your data

Veil has a few online features: shared capes (from 1.6.0), and friends, messages and invites (from 1.7.0). They
run on the Veil server, which runs on Cloudflare at `veil-server.veilclient.workers.dev`.

- **Friends:** add friends by their Minecraft name in **Social** or in the Veil launcher; they need to have used
  Veil once. Friends see when you're online and in game, and with **Show Server** on (Friends settings), which
  server. Servers you joined by IP address are never shown.
- **Messages:** only between friends, in Social and in the launcher. They're kept on the Veil server for 30 days,
  then deleted. You can report someone from your conversation; a report includes your last messages with them so
  TheDarkTeri can look at what happened.
- **Invites:** on a server, invite an online friend from your conversation; they click to join. Invites aren't
  stored.
- **Capes:** other Veil players see your Veil cape and you see theirs. A custom `cape.png` never leaves your PC;
  others see the Veil design in your color instead. To show capes, the mod asks the Veil server which players
  around you have one, by their Minecraft UUIDs.
- **Signing in:** the mod and the launcher prove who you are with the key Minecraft itself uses for signed chat
  and your public Mojang profile. Your Minecraft login, password and session token never go to Veil.
- **What the Veil server stores:** your Minecraft UUID and name, when you first and last signed in, your cape
  settings, your friends and friend requests, messages from the last 30 days, and reports. Whether you're online
  is never stored. Veil doesn't save your IP address (Cloudflare, which hosts the server, keeps short-lived request
  logs). Nothing is sent to the Minecraft servers you play on.
- **Turning it off:** turn off the **Friends** module to stop connecting for friends and messages (friends then
  see you offline, unless the Veil launcher is open). In the Cape settings, **Share** off removes your cape from
  the server and **Show Others** off stops looking up other players. With Friends off and no cape shared, the mod
  doesn't connect to Veil at all.
- **Deleting your data:** email [thedarkteriyt@gmail.com](mailto:thedarkteriyt@gmail.com) with your Minecraft
  name and everything stored about you, friends and messages included, is deleted.

### Server rules

Each server has its own rules about which mods are allowed. Veil only includes fair-play features, but it is up to
you to follow the rules of the servers you play on.

## Bugs and ideas

Found a bug or have an idea? Open an [issue](https://github.com/TheDarkTeri/Veil-Client-Releases/issues). For a
crash, attach the crash report from `.minecraft/crash-reports`. For anything else, email
[thedarkteriyt@gmail.com](mailto:thedarkteriyt@gmail.com).

## License

Copyright (c) 2026 TheDarkTeri. All rights reserved. You may download official releases and use them for personal
play. Copying, modifying, re-uploading or redistributing Veil Client needs written permission. See
[LICENSE](LICENSE).

Veil Client is made and maintained by TheDarkTeri, who is responsible for it
([thedarkteriyt@gmail.com](mailto:thedarkteriyt@gmail.com)). It is not affiliated with or endorsed by Mojang Studios,
Microsoft, Hypixel or Discord.
