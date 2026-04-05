# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A **mAirlist scripting language** (`.mls`) script that integrates the **Behringer CMD MM-1**
MIDI controller with [mAirlist](https://www.mairlist.com/) broadcast automation software
for voice tracking. Written in 2014.

**Key file:**
- `Behringer_CMD_MM-1.mls` — the single script; install by placing it in mAirlist's script folder

## Setup

1. Place `Behringer_CMD_MM-1.mls` in your mAirlist scripts folder (e.g. `C:\Program Files\mAirlist\scripts`)
2. Set `DEBUG = true`, run once from mAirlist, note the MIDI device number in the System Log
3. Set `mAirlistDevice` to the noted number
4. Optionally adjust the MIDI channel if buttons don't respond (use Behringer's app to check)
5. Set `DEBUG = false`
6. Configure the script as a **Notification Script** in mAirlist

## Notes

- This is a single-file, archived project with no active development since 2014
- The `.mls` format is mAirlist's proprietary scripting language (Pascal-like)
- MIDI channel and device number must be set per installation
