# Behringer CMD MM-1 for mAirlist

> **Archived** — Written in 2014 as a learning project; kept for nostalgic reasons. No active development.

A [mAirlist](https://www.mairlist.com/) notification script (`.mls`) that integrates the **Behringer CMD MM-1** MIDI controller for voice tracking workflows. Button LEDs and VU meters reflect player states in real time.

Inspired by [Behringer-CMD-LC-1](https://github.com/Lexorius/Mairlist-Behringer-Controller/blob/master/Behringer-CMD-LC-1.txt) by Thomas "Kloppi" Kloppholz.

---

## Requirements

- [mAirlist](https://www.mairlist.com/) broadcast automation software
- Behringer CMD MM-1 MIDI controller

---

## Installation

1. Copy `Behringer_CMD_MM-1.mls` into your mAirlist scripts folder, e.g.:
   ```
   C:\Program Files\mAirlist\scripts\
   ```

2. Open the script and set `DEBUG` to `true`:
   ```pascal
   DEBUG = true;
   ```

3. Run the script once from mAirlist. Open the **System Log** and note the device number of your controller.

4. Set `mAirlistDevice` to that number:
   ```pascal
   mAirlistDevice = 2;  // replace with your device number
   ```

5. Run the script again. All buttons should blink blue and the VU meters should light up to roughly 2/3.
   - If nothing happens, the MIDI channel may be wrong. Check/adjust `MIDICHANNL` in the script. You can use Behringer's app (available on their product page) to verify the channel.

6. Set `DEBUG` back to `false`:
   ```pascal
   DEBUG = false;
   ```

7. *(Optional)* Run the script once more with `DEBUG = false` to exit test mode and reset the LEDs.

8. Register the script as a **Notification Script** in mAirlist settings.

---

## LED behaviour

| Player state | Cue button | Side buttons |
|---|---|---|
| Loaded / Paused | Solid blue | Solid blue |
| Playing | Blinking blue | — |
| EOF warning | — | Blinking blue |
| PFL active | — | Blinking blue |
| Empty | Amber (off) | Amber (off) |

---

## License

Copyright 2014 Henning Halfpap. Licensed under the [Apache License 2.0](LICENSE.md).
