# Aliens: Fireteam Elite Save Editor (PS4/PC)

A save editor for *Aliens: Fireteam Elite* on PS4 and PC. Built in C# and WPF (.NET), this tool provides a comprehensive suite for editing character progression, weapons, attachments, appearances, emotes, intel, achievements, resources, and more.

---

## 🚀 Key Features

### 📂 File Handling
- **PC & PS4 Support:** Open and save both `char.sav` (PC) and `ue4savegame.ps4.sav` (PS4) files, with automatic XOR encoding/decoding applied transparently.
- **Quick Access:** Open your PC save folder or game folder directly from the editor. Automatically detects your Steam account — prompts you to choose if multiple accounts are found.
- **Save As:** Write to a new path without overwriting your original.
- **Unsaved Changes Warning:** Prompts before opening a new file if there are pending edits.

### 📈 Player Stats (Tab 1)
Edit your core character profile:
- **Account Level & XP** — Set your doc level and experience points.
- **Prestige Level, Prestige XP, and Last Claimed Prestige.**
- **Resources** — Set Credits and Rep Scrip to any amount.
- **Difficulty** — Set your last used and max unlocked difficulty.
- **Hardcore Mode** — Toggle the hardcore flag.
- **Max Buttons** — One-click max for account level, prestige, and resources.

### ⚔️ Classes (Tab 2)
Manage all character classes:
- View and edit **Level and XP** for each class individually.
- **Max Class** — Max the selected class in one click.
- **Max All Classes** — Max every class at once.
- **Add / Remove Recon** — Unlock or remove the hidden Recon class, with proper save data scaffolding generated automatically.

### 🔫 Weapons (Tab 3)
Full weapon inventory management, organized by category (Rifle, CQW, Hand Gun, Heavy):
- **Own / Unown** any weapon via checkbox — starter weapons are permanently locked to owned.
- Edit **Level and XP** per weapon.
- **Max Weapon / Max All Owned Weapons** — one-click max buttons.
- **Unlock All / Lock All** — bulk toggle ownership across all weapons.
- Live owned/total counter on each sub-tab header.

### 🔧 Attachments (Tab 4)
Full attachment inventory management, organized by slot (Armature, Barrel, Magazine, Muzzle, Optics):
- **Own / Unown** any attachment via checkbox.
- **Unlock All / Lock All** — bulk toggle.
- Live owned/total counter on each sub-tab header.

### 🧪 Consumables (Tab 5)
- Set quantities for all consumable items individually.
- **Max / Max All** — set one or all consumables to 999.
- **Clear All** — zero out all consumable stacks.

### 🃏 Challenge Cards (Tab 6)
- Set quantities for all challenge cards individually.
- **Max / Max All** — set one or all to 999,999,999.
- **Clear All** — zero out all challenge card stacks.

### 🎽 Appearances (Tab 7)
Manage cosmetic unlocks, organized by type (Outfits, Head Accessories, Weapon Colors, Weapon Decals):
- **Own / Unown** any appearance via checkbox — default appearances are permanently locked.
- **Unlock All / Lock All** — bulk toggle.
- Live owned/total counter on each sub-tab header.

### 🕺 Emotes (Tab 8)
- **Own / Unown** any emote via checkbox — default emotes are permanently locked.
- **Unlock All / Lock All** — bulk toggle (defaults are preserved on lock).
- Live owned/total counter.

### 📋 Intel (Tab 9)
Manage all discoverable intel, organized by campaign chapter (UAS Endeavor, Priority One, Giants in the Earth, The Gift of Fire, The Only Way to be Sure, Promise of a Flower):
- **Own / Unown** any intel entry via checkbox.
- **Unlock All / Lock All** — bulk toggle per chapter or globally.
- Live owned/total counter on each chapter sub-tab.

### 🏆 Achievements (Tab 10)
- View all achievements with their descriptions.
- Toggle individual achievements unlocked or locked.
- **Unlock All / Lock All** — bulk toggle.
- Live unlocked/total counter.

### 🔓 Misc / Content Unlocks (Tab 11)
Toggle special content unlock flags:
- **Hardcore Tiering**
- **Hardcore Character Creation**
- **Prestige Mode**

### 🔁 Save Converter
Seamlessly convert save files between platforms:
- **PS4 → PC:** Copy a PS4 save as a PC-compatible file.
- **PC → PS4:** Copy a PC save as a PS4-compatible file.

### 📄 Raw JSON
- **View** the full decoded JSON of your save at any time.
- **Export** the decoded JSON to a `.json` file for manual inspection or editing.
- **Import** a `.json` file back into the editor and repopulate all tabs automatically.

---

## 📝 How to Use

1. **Open:** Click *Open PS4 Save*, *Open PC Save*, or drag a `char.sav` / `ue4savegame.ps4.sav` file into the dialog.
2. **Edit:** Navigate the tabs to modify stats, inventory, weapons, appearances, and more.
3. **Save:** Click **Save File** to write changes back. The file is re-encoded automatically.
