# APublicizer

A small, practical **publicizer** toolchain for SCPSL / EXILED modding workflows — built to help you generate “publicized” assemblies for easier referencing, reflection, and development.

This repository primarily ships **ready-to-run binaries** inside the `APublicizer/` folder, so you can use it immediately without building from source.

---

## What it does

APublicizer is intended to take existing assemblies (e.g. game/mod assemblies) and produce **publicized** versions (e.g. `*-Publicized.dll`) so that otherwise-inaccessible members become easier to work with during plugin development.

You’ll see outputs like:

- `Assembly-CSharp.dll` → `Assembly-CSharp-Publicized.dll`
- `Exiled.API.dll` → `Exiled.API-Publicized.dll`

---

## Included

Inside `APublicizer/` you’ll find:

- `APublicizer.exe` — the executable
- Supporting runtime files (`.deps.json`, `.runtimeconfig.json`, etc.)
- Dependencies (e.g. Cecil-related DLLs)
- Example / produced outputs (e.g. `Assembly-CSharp-Publicized.dll`, `Exiled.API-Publicized.dll`)
- Helper batch scripts:
  - `@@StartSCPSL.bat`
  - `@@StartEXILED.bat`

---

## Quick start

### 1) Download / clone
Clone this repo or download it as a ZIP, then open the `APublicizer/` directory.

### 2) Run
Use one of the provided `.bat` scripts, or run the executable directly:

- Double-click `APublicizer.exe`, **or**
- Run `@@StartSCPSL.bat` / `@@StartEXILED.bat` depending on your workflow

> Tip: If you run into permission issues, try running the terminal as Administrator.

---

## Notes

- This repo currently looks like a **binary distribution** (no source project files in the root listing), so usage is focused on running the tool as-is.
- If you want, I can tailor this README to the *exact* CLI arguments / expected input-output paths once you tell me:
  - how `APublicizer.exe` is invoked (example command),
  - what folder it expects assemblies from,
  - where it writes results.

---

## License

See [`LICENSE`](./LICENSE).