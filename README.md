# Terra: Incognita — releases

**English** · [Русский](#русский)

This repository holds the files Terra Launcher downloads: the launcher installer, the signed
release documents and the modpack's files. It has no source code.

## Play

1. Download the newest `TerraLauncher-<version>-setup.exe` from
   [Releases](https://github.com/denfry/terra-incognita-releases/releases?q=launcher&expanded=true).
2. Run it. The installer is not yet signed with a certificate, so Windows SmartScreen shows
   *"Windows protected your PC"*: click **More info**, then **Run anyway**. The `.sha256` file next
   to the installer lets you check the download.
3. Open Terra Launcher, type the player name you want, press **PLAY**. The launcher installs Java,
   Minecraft, NeoForge and the pack itself (about 1.5 GB the first time), then starts the game.

Microsoft sign-in is not available yet: the launcher plays under the name you type. Singleplayer
works; a server lets such a player in only with `online-mode=false`. Sign-in arrives with a later
launcher version, and installed launchers update themselves.

Requirements: Windows 10/11 64-bit, 8 GB RAM (the game gets 6 GB), about 4 GB of disk.

## What is in here

| Where | What |
|---|---|
| Releases `launcher-v<version>` | the installer and its checksum |
| Releases `objects-00` … `objects-ff` | the pack's files, one asset per file, named by SHA-256 |
| branch `gh-pages` | the trust root, channel pointers and signed manifests the launcher reads |

Every file the launcher installs is named, with its hash, in a manifest signed by the project's
keys; the launcher trusts nothing else. Third-party mods keep their own licences; the launcher
downloads the ones whose licence does not allow redistribution straight from their authors.

---

## Русский

Здесь лежат файлы, которые скачивает Terra Launcher: установщик лаунчера, подписанные документы
релиза и файлы сборки. Исходного кода тут нет.

### Как играть

1. Скачайте свежий `TerraLauncher-<версия>-setup.exe` из
   [Releases](https://github.com/denfry/terra-incognita-releases/releases?q=launcher&expanded=true).
2. Запустите его. Установщик пока не подписан сертификатом, поэтому Windows SmartScreen покажет
   «Система Windows защитила ваш компьютер»: нажмите **Подробнее**, затем **Выполнить в любом
   случае**. Файл `.sha256` рядом с установщиком позволяет проверить скачанное.
3. Откройте Terra Launcher, впишите имя игрока, нажмите **PLAY**. Лаунчер сам поставит Java,
   Minecraft, NeoForge и сборку (около 1,5 ГБ в первый раз) и запустит игру.

Вход через Microsoft пока недоступен: лаунчер запускает игру под введённым именем. Одиночная игра
работает; на сервер такого игрока пустит только `online-mode=false`. Вход появится в следующей
версии лаунчера, установленные лаунчеры обновятся сами.

Требования: Windows 10/11 64-bit, 8 ГБ ОЗУ (игре достаётся 6 ГБ), около 4 ГБ на диске.
