# FIFA 14 fix for shadPS4

Unofficial [shadPS4](https://github.com/shadps4-emu/shadPS4) build with fixes for **FIFA 14 (CUSA00128, EUR, update 01.06)**, to be used with **shadPS4 Qt Launcher**.

> Not affiliated with or supported by the shadPS4 team. Please do not report problems with this build upstream.

**Download:** [latest release](../../releases/latest)

## What it fixes
- Missing pitch texture and the same grass in every stadium.
- Replays not playing (players frozen after a goal).
- Player names on the back of the jerseys missing or corrupted.
- Brightness (gamma) setting saved between sessions.
- Replays and cutscenes at 60 FPS (optional game patch, applied in memory).
- Correct bloom/glare in day and night/rain matches: real Vulkan occlusion queries instead of fake values.

## Installation
1. Download `FIFA14-fix.zip` from the [latest release](../../releases/latest).
2. Copy the `FIFA14-fix` folder to `%APPDATA%\shadPS4QtLauncher\versions\`.
3. In the launcher's **Version Manager**, add a custom version, select that `shadps4.exe` and name it **FIFA 14 fix**.
4. Copy `custom_configs\CUSA00128.json` to `%APPDATA%\shadPS4\custom_configs\`.
5. *(Optional, 60 FPS)* Copy `patches\FIFA14-fix` to `%APPDATA%\shadPS4\patches\`.

Full instructions: `README.txt` (English) and `LEEME.txt` (Spanish) inside the zip.

## Repository contents
| Path | |
|---|---|
| `patches/FIFA14-fix/` | 60 FPS replays/cutscenes game patch (shadPS4 XML patch format) |
| `source/fifa14-fix.patch` | Full diff against shadPS4 `b72489d` |

The complete source tree is the [`fifa14-fix`](https://github.com/danilenko22/shadPS4/tree/fifa14-fix) branch of my shadPS4 fork.

## License
GPL-2.0, same as shadPS4 (see [LICENSE](LICENSE)). No game files, firmware, system modules or keys are included. You need your own dump of the game.
