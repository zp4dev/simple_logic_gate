# Simple Logic Gate in Digital Logic Sim

This project contains basic logic gates built with **Digital Logic Sim**, including:

- `AND.json`
- `OR.json`
- `NOT.json`
- `NOR.json`
- `XNOR.json`

## Requirements

- **Digital Logic Sim** installed (Windows / Linux / macOS).
- At least one **project** already created inside the app (open the app and create a new project if you don't have one yet).

## Chip save folder location by OS

Digital Logic Sim stores project data (including chips/logic gates) inside Unity's data folder, under the project you created in the app:

| OS | Path |
|---|---|
| **Windows** | `C:\Users\<username>\AppData\LocalLow\Sebastian Lague\Digital Logic Sim\SaveData\<Project_Name>\Chips` |
| **Linux** | `~/.config/unity3d/Sebastian Lague/Digital Logic Sim/SaveData/<Project_Name>/Chips` |
| **macOS** | `~/Library/Application Support/Sebastian Lague/Digital Logic Sim/SaveData/<Project_Name>/Chips` |

> Note: the subfolder name (e.g. `Chips`) may differ slightly depending on the app version you're using. If it doesn't match exactly, try creating a simple chip inside the app first and locate the saved file to confirm the correct path.

## How to load the logic gate files into the app

### General steps (applies to all three OSes)

1. Open **Digital Logic Sim**, create or open a project (e.g. name it `Simple logic gate in digital logic sim`).
2. Fully close the app to avoid conflicts while copying files.
3. Copy the 5 files `AND.json`, `OR.json`, `NOT.json`, `NOR.json`, `XNOR.json` into the correct `Chips` folder of that project (see path table above).
4. Reopen the app and go into the project you just edited. The `AND`, `OR`, `NOT`, `NOR`, `XNOR` gates will now appear in the list of available chips.

### Windows

1. Press `Windows + R`, type `%AppData%\..\LocalLow\Sebastian Lague\Digital Logic Sim\SaveData`, then press Enter.
2. Navigate to your project folder, then into the `Chips` folder.
3. Copy the 5 `.json` files there.

### Linux

1. Open a terminal and run:
   ```
   cd ~/.config/unity3d/"Sebastian Lague"/"Digital Logic Sim"/SaveData
   ```
2. Navigate to your project folder, then into the `Chips` folder.
3. Copy the 5 `.json` files there, for example:
   ```
   cp AND.json OR.json NOT.json NOR.json XNOR.json "<Project_Name>/Chips/"
   ```

### macOS

1. Open Finder, press `Cmd + Shift + G`, and type:
   ```
   ~/Library/Application Support/Sebastian Lague/Digital Logic Sim/SaveData
   ```
2. Navigate to your project folder, then into the `Chips` folder.
3. Copy the 5 `.json` files there.

## Verifying after loading

- Open the app and load the project you copied the files into.
- Check the chip list (usually in the bottom-left corner) to confirm all 5 gates — AND, OR, NOT, NOR, XNOR — appear.
- If they don't show up, try restarting the app or double-check that you used the correct project path.

## Notes

- Back up your `SaveData` folder before overwriting any files, to avoid losing existing project data.
- Keep the file names exactly as they are (`AND.json`, `OR.json`, etc.) so they match the chip names used inside the app.
