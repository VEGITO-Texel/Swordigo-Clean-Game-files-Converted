The Developer Of this Project is------------https://github.com/TheCorrectSynovian
# 🗡️ Swordigo - Clean Game Files & Converted Assets

Cleaned, extracted, and pre-configured assets for the **Swordigo Windows Portable Edition** (AevoraLabs project). This repository provides ready-to-use game files, converted audio assets, and a portable launcher setup.

---

## 🌟 Features & Fixes Included

- **Cleaned Asset Structure:** Converted audio tracks and assets properly mapped for the engine.
- **100% Portable Setup:** Pre-configured `swordfare.bat` script that redirects `%APPDATA%` saves to a local `data/` folder inside the game directory. Your save files stay safe even if you format Windows!
- **Asset Viewer Ready:** Fully compatible with `Ruby.exe` for viewing assets and scene tools.
- **Pre-packaged DLLs:** Includes all necessary runtime binaries (`SDL3`, `OpenAL`, `GLEW`, `vorbis`, `mpg123`, `zlib`, etc.) for 64-bit Windows 10/11.

---

## 🚀 How to Run

1. **Download / Clone** this repository to your PC.
2. Open the project folder.
3. Launch the game using **`swordfare.bat`** (or `swordfare.exe`).
   > 💡 **Tip:** Always use `swordfare.bat` if you want your save files stored inside the `data/` folder in the game directory instead of `%APPDATA%`.

---

## 📂 Folder Structure Overview

Swordigo-Clean-Game-files-Converted/
├── assets/             # Game assets (textures, audio, scenes)
├── engine/             # Engine dependencies and core scripts
├── external/           # Third-party libraries
├── launcher/           # Launcher binaries
├── res/                # Game resources
├── data/               # Local portable saves (created on launch)
├── swordfare.exe       # Main game executable
├── swordfare.bat       # Portable launcher script (Recommended)
├── Ruby.exe            # Asset viewer / Scene tool
└── *.dll               # Required runtime DLLs

---

## ⚙️ Portable Save Data Details

By default, the game engine attempts to read/write saves from `%APPDATA%\swordigo-desktop\`. 

Using **`swordfare.bat`** redirects the save directory to:
`./data/swordigo-desktop/`

This ensures:
- Easy backup and transfer to other PCs / USB drives.
- Progress won't be lost during Windows reinstallations.

---

## 📝 Notes & Troubleshooting

- **Micro-stutters during level transitions:** Happens due to real-time GLSL shader compilation (especially on AMD GPUs) and synchronous asset loading in dev builds. Installing on an **SSD** significantly reduces this delay.
- **Asset Editing:** Use `Ruby.exe` to inspect scenes and verify audio asset paths.

---

## ❤️ Credits & Thanks


- **Touch Foo** — Original creators of *Swordigo*.

- 
- **AevoraLabs Team** — For developing the open-source Windows engine port and tools.

- 
- **VEGITO-Texel** — Clean asset conversion, audio fixes, and portable configuration.

- 
- **QuantumCreeper -- Developer Of AevoraLabs Projects

- 
- **Mr Sinups-The Contributor of AevoraLabs Project
- 
- 
-**Reallinusweiss-The Developer of Aevoralabs in Windows Porting

  
*Disclaimer: This repository is intended for modding, testing, and archival purposes.*
