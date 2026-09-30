# MetrosHome 🏠✨

A polished, GUI-driven home system. `/home` opens a clean chest menu with clickable home slots instead of a wall of text — teleport, create, and delete homes without ever memorizing IDs. 🕵️‍♂️

---

## 🚀 Features 🌟

- 🖥️ **`/home`** → opens a 4-row GUI with home slots laid out horizontally, delete buttons underneath
- 🛏️ Filled slots show a pink bed (click to teleport) with a matching pink dye below (click to delete)
- ⬜ Empty slots show a light-gray bed/dye (click to instantly create a home there)
- 🔒 Locked slots (past your rank's limit) show red bed/dye with a clear "upgrade for more" message
- ✅ **Delete confirmation GUI** — red glass to cancel, lime glass to confirm, home preview in the center — no accidental deletes
- ⏳ **Configurable teleport warmup**, cancels automatically if you move, bypassable via permission
- 🔊 Full sound feedback for every action — open, teleport, create, delete, cancel
- 💾 **SQLite-backed persistence** — homes survive restarts, loaded/saved asynchronously so it never causes lag
- 🎚️ **Permission-based home limits** — default, VIP, premium, elite, and unlimited tiers, all configurable
- 🏷️ Named homes supported via `/sethome <name>` alongside the numbered GUI slots
- 🚫 Blockable worlds — prevent home creation in specific dimensions/maps
- 🧩 Every GUI title, item, color, lore line, and message is editable in `config.yml` — no recompiling needed

---

## 📜 Commands

| Command                     | Description                                  |
| ----------------------------- | ----------------------------------------------- |
| `/home` `/homes`             | 🖥️ Open the homes GUI                          |
| `/home <id>`                 | 🌀 Teleport straight to that home                |
| `/sethome`                   | ➕ Create a home in the next free numbered slot  |
| `/sethome <name>`            | 🏷️ Create a named home                          |
| `/delhome <id/name>`         | ❌ Delete a home                                 |
| `/renamehome <old> <new>`    | ✏️ Rename an existing home                       |

## 🔑 Permissions

| Permission             | Description                          |
| ----------------------- | --------------------------------------- |
| `homes.default`         | Base home limit (everyone)             |
| `homes.vip`             | VIP home limit tier                    |
| `homes.premium`         | Premium home limit tier                |
| `homes.elite`           | Elite home limit tier                  |
| `homes.unlimited`       | No home limit                          |
| `homes.bypasswarmup`    | Skip the teleport countdown entirely   |

## ⚙️ Configuration

Everything is editable in `config.yml`: GUI title & slot positions, home limits per tier, teleport warmup & movement-cancel behavior, blocked worlds, every item's material/name/lore, every message, and every sound.

Found at `plugins/MetrosHome/config.yml` after first run.

---

## ⚡ Installation

1. Download the latest JAR and place it in your server's `plugins` folder 📥
2. Start or restart your Paper server 🔄
3. Tune `config.yml` to match your server's rank structure

**Requires:** Paper 1.21.11+ • Java 21+

---

## 📄 Author & Use

Plugin by **Metro** 💥
Free to use on your servers. Re-uploading or claiming as your own is **not allowed**.

---

Home, but make it clickable. 🎉🏠
