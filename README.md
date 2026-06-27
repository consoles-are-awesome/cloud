<p align="center">
  <img src="powerplay/resources/icon/icon_load.gif" alt="PowerPlay Icon" width="96" />
</p>

<h1 align="center">Consoles-are-Awesome: Cloud</h1>

<p align="center">
  Static support files for <b>PowerPlay</b>, a desktop companion app for <b>Team Fortress 2
   
  </b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/type-public_static_storage-ff4fd8?style=for-the-badge&labelColor=04070f" alt="Type: public static storage" />
  <img src="https://img.shields.io/badge/app-PowerPlay-00ffff?style=for-the-badge&labelColor=04070f" alt="PowerPlay" />
  <img src="https://img.shields.io/badge/game-Team_Fortress_2-fff3b0?style=for-the-badge&labelColor=04070f" alt="Team Fortress 2" />
</p>

---

## What this is

This repository is a lightweight public file host for remote resources used by **PowerPlay**.

It allows for dynamic content like broadcasted "Server Messages" to be updated in real-time in the PowerPlay app without actually updating the program's source code.
Among other features, it also supplies unique SteamID lists for various features such as Tester Whitelisting, Community Recognition, and Item Ownership tracking.

## What it is used for

PowerPlay may reference this repo for public data such as:

- community and badge-related Steam3ID lists
- app helper text
- Quickplay server-lists
- public icon/helper assets
- remote system-message data

## Repository layout

```text
.
├─ powerplay/
│  ├─ community/          Public TF2 community Steam3ID lists
│  ├─ helpers/            Small helper text/assets used by PowerPlay
│  ├─ quickplay/servers/  Quickplay server lists by category
│  ├─ resources/icon/     Public PowerPlay icon assets
│  └─ server_message.json Remote message payload for quick notices
└─ README.md
```

## File format notes

Most list files are plain text and intentionally simple.  
Steam user list entries are required to be seperated by newlines using the Steam3ID format. Commented lines are ignored by the app.

`server_message.json` is used for quick app-facing announcements.

`SIG.dat` is a file whose contents PowerPlay treats as the current "signature". This can prepend various chat messages, assist with user echo cancellation, and allows for self-identify to function.

## Contributing

Corrections, cleanup, and list updates are welcomed through issues or pull requests!
