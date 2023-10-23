# Installation Server

## 1. Verzeichnis vorbereiten

Gehe im Terminal zum Ort, an dem sie denn Server installieren wollen.&#x20;

## 2. Git-Repo clonen

```bash
git clone https://github.com/KidsLabDe/zfn-server-docker
```

## 3. Tutorial Server starten

```bash
sudo ./startTutorial.sh
```

<details>

<summary>Ausgabe Terminal</summary>

```log
minetest_zfn  | ───────────────────────────────────────
minetest_zfn  | 
minetest_zfn  |       ██╗     ███████╗██╗ ██████╗ 
minetest_zfn  |       ██║     ██╔════╝██║██╔═══██╗
minetest_zfn  |       ██║     ███████╗██║██║   ██║
minetest_zfn  |       ██║     ╚════██║██║██║   ██║
minetest_zfn  |       ███████╗███████║██║╚██████╔╝
minetest_zfn  |       ╚══════╝╚══════╝╚═╝ ╚═════╝ 
minetest_zfn  | 
minetest_zfn  |    Brought to you by linuxserver.io
minetest_zfn  | ───────────────────────────────────────
minetest_zfn  | 
minetest_zfn  | To support LSIO projects visit:
minetest_zfn  | https://www.linuxserver.io/donate/
minetest_zfn  | 
minetest_zfn  | ───────────────────────────────────────
minetest_zfn  | GID/UID
minetest_zfn  | ───────────────────────────────────────
minetest_zfn  | 
minetest_zfn  | User UID:    1000
minetest_zfn  | User GID:    1000
minetest_zfn  | ───────────────────────────────────────
minetest_zfn  |          __.               __.                 __.  
minetest_zfn  |   _____ |__| ____   _____ /  |_  _____  _____ /  |_ 
minetest_zfn  |  /     \|  |/    \ /  __ \    _\/  __ \/   __>    _\
minetest_zfn  | |  Y Y  \  |   |  \   ___/|  | |   ___/\___  \|  |  
minetest_zfn  | |__|_|  /  |___|  /\______>  |  \______>_____/|  |  
minetest_zfn  |       \/ \/     \/         \/                  \/   
minetest_zfn  | 2023-10-23 08:53:33: ACTION[Main]: World at [/config/.minetest/worlds/Tutorial]
minetest_zfn  | 2023-10-23 08:53:33: ACTION[Main]: Server for gameid="antigrief" listening on 0.0.0.0:30000.
minetest_zfn  | Unified Inventory. Inventory size: 1333


```

</details>

## 4. Verbindung testen

* Starte Minetest
* Wechsle zum Reiter `Spiel beitreten`
  * Adresse: `localhost`
  * Port: `30000`
  * Name: `Mentor`
  * Passwort: `zukunft`
