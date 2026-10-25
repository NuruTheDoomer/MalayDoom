## Overview

MalayDoom aims to support a broad range of Doom source ports, covering both classic ports and ports with extended or port-specific features.

This page records the localization features tested across different ports and versions, including DeHackEd/BEX text mnemonics and menu graphics. Compatibility may vary between ports and versions.

> **Last updated: 25th October 2026**

## Main Compatibility Table

This table provides an overview of MalayDoom's compatibility across the tested source ports and their localization features.

The test is done using the following ports:

Chocolate Doom v3.1.1, Crispy Doom v7.1.0, PrBoom+ v2.6.66, PrBoomX v2.9.2, DSDA-Doom v0.28.2 & v0.30.0, Nyan Doom v1.2.4 & v1.6.0, Woof v15.3.0 & v16.0.0, Nugget Doom v5.1.0 & v6.0.1, Cherry Doom v2.1.0, UZDoom v5.0.1, Eternity Engine v4.06.00, Russian Doom (Win) v6.3, ZDoom 2.8.1, LZDoom v4.14.4, Boom v2.02, MBF v2.03, Russian Doom (DOS) v1.8

| Status | Meaning                                                                                                                                                                           |
|:------:| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Y      | Modifiable and tested                                                                                                                                                             |
| N      | Not modifiable                                                                                                                                                                    |
| P      | Partially modifiable                                                                                                                                                              |
| S      | Planned to be modifiable / is modifiable in development versions                                                                                                                  |
| R      | Removed / not modifiable in latest port versions<br/>See the **Version-Specific Differences** section below.                                                                      |
| A      | Alternative - This string/feature may have alternative mnemonic(s), either through DeHackEd/BEX or another lump such as `LANGUAGE`, that is not currently supported by MalayDoom. |
| ?      | Not tested                                                                                                                                                                        |
| -      | Not applicable                                                                                                                                                                    |

| Feature(s)                                                     | Chocolate | Crispy | PrBoom+ | PrBoomX | DSDA | Nyan   | Woof!  | Nugget | Cherry | UZDoom | Eternity | Russian Doom (Win) | ZDoom | LZDoom | Boom (DOS) | MBF (DOS) | Russian Doom (DOS) |
|:-------------------------------------------------------------- |:---------:|:------:|:-------:|:-------:|:----:|:------:|:------:|:------:|:------:|:------:|:--------:|:------------------:|:-----:|:------:|:----------:|:---------:|:------------------:|
| Level Name Graphics                                            | Y         | Y      | Y       | Y       | Y    | Y      | Y      | Y      | Y      | Y      | Y        | Y                  | Y     | Y      | Y          | Y         | Y                  |
| (Vanilla) Menu Graphics                                        | Y         | Y      | Y       | Y       | Y    | Y      | Y      | Y      | Y      | Y      | Y        | Y                  | Y     | Y      | Y          | Y         | Y                  |
| (Vanilla) Options Menu Graphics                                | Y         | Y      | Y       | Y       | R    | R      | -      | -      | -      | -      | -        | -                  | -     | -      | Y          | Y         | -                  |
| (Boom) Options Menu Graphics                                   | -         | -      | Y       | Y       | R    | R      | Y      | Y      | Y      | -      | -        | -                  | -     | -      | Y          | Y         | -                  |
| (Port-specific) Menu Graphics                                  | -         | Y      | -       | -       | R    | Y**¹** | Y      | Y      | Y      | -      | P*       | N**²**             | -     | Y      | -          | -         | Y                  |
| (Crispy Doom) Doom II Expansion Episode Graphics               | -         | Y      | -       | -       | -    | -      | -      | -      | -      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| ENDOOM/ENDBOOM                                                 | Y         | Y      | Y       | Y       | Y    | Y      | Y      | Y      | Y      | Y      | Y        | Y                  | Y     | Y      | Y          | Y         | Y                  |
| Widescreen Assets / Status Bar (16:9)                          | -         | Y      | Y       | Y       | Y    | Y      | Y      | Y      | Y      | Y      | Y        | Y                  | N     | Y      | -          | -         | -                  |
| Message Line Wrapping                                          | N         | N      | N       | N       | N    | Y      | N      | N      | N      | Y      | N        | N                  | N     | N      | N          | N         | N                  |
| Text Screen Line Wrapping                                      | N         | Y      | N       | N       | N    | N      | N      | N      | N      | N      | N        | N                  | N     | N      | N          | N         | N                  |
| UMAPINFO                                                       | -         | Y      | Y       | Y       | Y    | Y      | Y      | Y      | Y      | Y      | Y        | -                  | -     | -      | -          | -         | -                  |
| BEX's [STRING] Mnemonics                                       | Y**³**    | Y      | Y       | Y       | Y    | Y      | Y      | Y      | Y      | Y      | Y        | Y                  | Y     | Y      | Y**³**     | Y         | Y                  |
| QUITMSG                                                        | Y         | Y      | N       | N       | N    | N      | Y      | Y      | Y      | Y      | Y        | Y                  | Y     | Y      | N          | N         | N                  |
| QUITMSG1-14                                                    | N         | N      | N       | N       | Y    | Y      | Y      | Y      | Y      | Y      | -        | N                  | Y     | Y      | N          | N         | N                  |
| "Press Y to Quit." text (DOSY)                                 | N         | N      | Y       | Y       | Y    | Y      | R      | R      | Y      | Y      | Y        | N                  | Y     | Y      | Y          | Y         | N                  |
| Secret revealed notification (HUSTR_SECRETFOUND)               | -         | N      | N       | N       | Y    | Y**⁴** | Y**⁴** | Y**⁴** | Y**⁴** | A      | N        | A                  | A     | A      | -          | -         | A                  |
| Alternate secret revealed notifications (Count, Percentage...) | -         | -      | -       | -       | -    | N      | N      | N      | N      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| Milestone notifications                                        | -         | -      | -       | -       | -    | N      | N      | N      | N      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| Evil Sceptre & Unholy Bible pickup message (BETA_BONUS3/4)     | -         | Y      | -       | -       | Y    | Y      | Y      | Y      | Y      | A      | Y        | A                  | A     | A      | -          | -         | A                  |
| "Empty Slot" text (EMPTYSTRING)                                | N         | N      | Y       | Y       | Y    | Y      | Y      | Y      | Y      | -      | -        | -                  | -     | -      | Y          | Y         | -                  |
| "Gamma Correction Level" text (GAMMALVL)                       | Y         | Y      | Y       | Y       | Y    | Y      | N      | N      | N      | -      | Y        | A                  | A     | A      | Y          | Y         | A                  |
| Extended GAMMALVL ranges                                       | -         | N      | -       | -       | -    | -      | N      | N      | N      | -      | -        | A                  | A     | A      | -          | -         | -                  |
| Automap: Overlay Mode (AMSTR_OVERLAY*)                         | -         | Y      | N       | N       | N    | N      | Y      | Y      | Y      | -      | N        | N                  | -     | -      | -          | -         | -                  |
| Automap: Dark Overlay                                          | -         | -      | -       | -       | N    | N      | N      | N      | N      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| Automap: Rotate Mode (AMSTR_ROTATE*)                           | -         | Y      | N       | N       | N    | N      | Y      | Y      | Y      | -      | -        | N                  | -     | -      | -          | -         | N                  |
| Automap: Textured Mode (AMSTR_TEXTURE*)                        | -         | -      | N       | N       | N    | N      | -      | -      | -      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| Obituaries (OB_\*)                                             | -         | -      | -       | -       | -    | Y      | Y      | Y      | Y      | Y      | -        | -                  | -     | -      | -          | -         | -                  |
| SIGIL I/II level names (HUSTR_E5M*/E6M*)                       | -         | N      | -       | -       | -    | -      | -      | -      | -      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| Xbox E1M10 level name (HUSTR_E1M10)                            | -         | N      | -       | -       | -    | -      | -      | -      | -      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| John Romero's E1M4B & E1M8B level names (HUSTR_E1M4B/E1M8B)    | -         | N      | -       | -       | -    | -      | -      | -      | -      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| Xbox MAP33 level name (HUSTR_33)                               | -         | -      | -       | Y       | -    | -      | -      | -      | -      | -      | -        | -                  | -     | -      | -          | -         | -                  |
| Master Levels & NRFTL level names (MHUSTR_\* / NHUSTR_\*)      | -         | N      | -       | -       | -    | -      | -      | -      | -      | -      | -        | -                  | -     | -      | -          | -         | -                  |

**1** = Some menu graphics exclusive for this port were removed, while some are still in use, see the **Port-Specific Graphics** section below

**2** = The custom `M_UNMARE` graphic does not load in the Windows version of Russian Doom but does in the DOS version

**3** = Requires the separate deh file (or `-dehlump` parameter for Chocolate Doom)

**4** = Nyan: Secret Message Format must be set to `Default`; Woof/Nugget/Cherry: Announce Revealed Secrets must be set to `On`

***** = See the [Not Supported](#not-supported) section below

---

## Port-Specific Graphics

| Lump Name  | In-Game Name/Label | Currently Used in                                   | No Longer Used in                          |
|:----------:| ------------------ | --------------------------------------------------- | ------------------------------------------ |
| `M_CRISPY` | Crispness          | Crispy Doom                                         | -                                          |
| `M_CSTSKL` | Customize Skill... | Woof!<br/>Nugget Doom<br/>Cherry Doom<br/>Nyan Doom | -                                          |
| `M_EXTR`   | Unholy Massacre    | LZDoom                                              | -                                          |
| `M_GAMEPL` | Gameplay / Demos   | -                                                   | Nyan Doom (1.2.5+)                         |
| `M_LVLTBL` | Level Table        | Cherry Doom                                         | DSDA-Doom (0.29.0+)<br/>Nyan Doom (1.2.5+) |
| `M_UNMARE` | Ultra-Nightmare!   | Russian Doom**¹**                                   |                                            |

**1** = Currently doesn't show up in the Windows version of Russian Doom, but does in the DOS version

---

## Port-Specific Notes

Some ports require additional explanation due to their unique localization systems, configuration options, or other compatibility considerations. These details are documented here rather than in the main table.

---

## Version-Specific Differences

**DSDA-Doom v0.29.0** and **Nyan Doom v1.2.5** removed support for Boom's static menu graphic lumps for its options menu as part of their menu redesign, which favour more dynamic text rendering via DBIGFONT.... The reasoning behind the removal as stated by one of the devs is:

> The main problem with allowing graphics [in the options menu] is as menus change, some would not have replacement lumps... that's one of the reasons it was removed, is because you'd get a mix and match in wads to only replaced some graphics, while later versions would be missing graphics.

... which makes sense. In versions 0.25 through 0.28 of DSDA-Doom, if the `M_LVLTBL` lump is not provided by a wad then ALL the options in the menu falls back to NOT use these graphics lumps, while still allowing those graphics to appear as menu titles in their respective submenus.

Another removal is the `DOSY` BEX mnemonic (the "Press Y to quit" text) support in **Woof! v16.0.0** and **Nugget Doom v6.0.0**.

The affected lumps and mnemonics are still kept in the wad files in case some other ports also use the same lumps and/or mnemonics. For example, Cherry Doom, a fork of Nugget Doom, still use Boom's static menu graphic lumps, and thus will use `M_LVLTBL` for the Level Table Menu option.

---

## MIDI Pack Compatibility

Some MIDI packs use UMAPINFO to redefine music assignments. One example is the Ultimate MIDI Pack, which used UMAPINFO to change the music lump that is used for all Episode 4 levels from the hardcoded, reused E1-E3 music to the new D_E4M* MIDI lumps made for the MIDI pack.

This method however affects MalayDoom due to the UMAPINFO definitions overriding the translated names that are implemented via BEX. And thus addon WADs is provided for the following MIDI packs:

| MIDI Pack                                                          | Addon Name               | Load Order / Command Line Parameters                                                                             |
| ------------------------------------------------------------------ | ------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| Ultimate MIDI Pack (ultimidi.wad)                                  | MalayDoom-ULTIMIDI.wad   | `-iwad doom.wad -file ultimidi.wad MalayDoom-Doom1.wad MalayDoom-ULTIMIDI.wad`                                   |
| Master Levels for Doom II 25th Anniversary MIDI Pack (KEX version) | MalayDoom-MLMIDI-KEX.wad | `-iwad doom2.wad -file masterlevels.wad ml_midipack_crispydoom.wad MalayDoom-Doom2.wad MalayDoom-MLMIDI-KEX.wad` |
| No Rest for the Living MIDI Pack                                   | MalayDoom-NRFTLMIDI.wad  | `-iwad doom2.wad -file nerve.wad nrftl_midipack_prboomplus.wad MalayDoom-Doom2.wad MalayDoom-NRFTLMIDI.wad`      |

The PSN version of Master Levels doesn't require a separate MIDI pack addon since there's no custom music assignments for any of the maps so you can just load it using the regular PSN Master Levels localization wad using the following command line parameters:
`-iwad doom2.wad -file masterlevels.wad ml_midipack_crispydoom.wad MalayDoom-Doom2.wad MalayDoom-MasterLevels-PSN.wad`

---

## DOS Compatibility and Legacy Ports

Since filenames in DOS are limited to 8 characters, a separate zip file is provided that changes the names of the following WADs:

- MalayDoom-Doom1.wad = MalayD1.wad

- MalayDoom-Doom2.wad = MalayD2.wad

- MalayDoom-TNT.wad = MalayTNT.wad

- MalayDoom-Plutonia.wad = MalayPLU.wad

- MalayDoom.deh = MalayDEH.deh*

\* = for use with the Boom source port, since it doesn't have the embedded DeHackEd lump support introduced in MBF

Vanilla Doom are also not supported since this project utilize Boom's BEX [STRINGS] mnemonics

## Not Supported

This section lists features or localization lumps that MalayDoom does not currently support.

- `LANGUAGE` lump, used in ZDoom-family ports and Helion
  
  - Any strings already exposed via BEX will be replaced, but others that are only exposed through `LANGUAGE` will not
  - Support for ZDoom's/Helion's LANGUAGE lumps may be introduced in a future revision

- The following hardcoded menu titles in Eternity Engine
  
  - Key Bindings: **Basic Movement**, **Advanced Movement**, **Weapon Keys**, **Inventory/Environment**, **Game Functions**, **Menu Keys**, **Automap**, **Console**
  
  - **Gamepad Settings**
  
  - **Configuration**

- Strings exclusive to some ports such as Russian Doom and Doom Retro. (may be added in a future revision)

---

## Untested Ports

These ports have not been tested with MalayDoom. An untested port should not be considered unsupported unless stated otherwise.

- Helion

- Doom Retro

- GZDoom

- Zandronum

- ZDaemon

- Odamex
