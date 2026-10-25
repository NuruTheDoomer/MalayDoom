# MalayDoom History

This page documents the history of the project, mostly from my own recollection, as it's been a long time since I first started working on it.

## 2021-2023

MalayDoom began around 2021 as a small fan-made side-project to translate Doom into Bahasa Melayu while working on other localization works. Initially I named it KetupatDoom, inspired by the [BaguetteDoom](https://www.doomworld.com/forum/topic/108152-baguettedoom-a-fanmade-french-translation-of-doom/) project which adds fanmade French translations to GZDoom... I also started making the project as a GZDoom wad, using the `LANGUAGE` lump (that is the old ZDoom format, not the newer CSV format) and all... But eventually I thought of making the project compatible with all the other source ports other than GZDoom so I restarted the project and started utilizing BEX instead, which is compatible with a lot more ports.

If you're wondering why I decided to make this project, it's because I was (and still am) part of the Minecraft translation team, as part of which I helped translate the game into Malay. And I think my interest in translating stuff into Malay somehow manifested in Doom as well, especially after seeing the BaguetteDoom project.

Among the earliest programs I used is [DoomWriter](https://github.com/Visual-Vincent/DoomWriter), which was used to generate the level name and menu graphics. Another tool is [WhackEd4](https://www.teamhellspawn.com/exl/whacked4/), which is a DeHackEd editor, but one thing about WhackEd is that whenever I added a mnemonic that is not one of Boom's STRINGS mnemonic, the program just crashes. So eventually I just moved on to use SLADE3 for DeHackEd editing instead, alongside the general WAD editing stuff.

The current scope at the time is all the four main IWADs, Master Levels, No Rest for the Living, and SIGIL.

## 2024

SIGIL II's level names and text got added to the project after it was released back in December, with Legacy of Rust's (and id Deathmatch Pack #1 (iddm1.wad)'s) level names and texts were also added following the Doom + Doom II release in August.

This is also around the time that I've decided to replace all the old level name and menu graphics made using DoomWriter to the ones generated using [eevee's Doom Text Generator](https://c.eev.ee/doom-text-generator/) website, which I must say is pretty handy!

## 2026

Around July/August, I've decided to start working on bringing the MalayDoom project past the initial finish line, that is Revision 1. Initially I wanted to target August 31st or September 16th (Malaysia's National Day and Malaysia Day respectively), but after some thinking, I thought that releasing Revision 1 of this project during the Bulan Bahasa Kebangsaan month (basically Malaysia's national language month) would be a better idea.

During this time the wad files for the expansions' translations are finalized, along with the MIDI Pack compatible addon for MIDI Packs that used UMAPINFO, since it will overwrite the level names implemented via BEX. Compatibility and differences in localization support between ports have also began to be documented, whether that is support for specific BEX mnemonics or support for specific graphic lumps.

Some of the translations are also finalized, with huge changes happening to some of the level names and, more notably, the intermission texts, with the goal of hopefully getting the translation to feel closer to the original material.

### Future Revisions

Future revisions of this project will hopefully include stuff like the full localized graphics for the title screens, credits screens, help screens, the game logo (M_DOOM), and support for more BEX mnemonics specific to some ports, as well as other localization lumps such as ZDoom's/Helion's `LANGUAGE` lump
