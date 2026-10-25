# MalayDoom Terminology

This page records the established terminology used throughout MalayDoom, along with notes explaining selected localization decisions. Please refer to these terms and guidelines when helping to review or improve the translations.

## General Terminology

MalayDoom uses consistent terminology for common Doom gameplay terms where appropriate.

| English                   | Malay               | Notes                                                                                                                        |
| ------------------------- | ------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Level                     | Tahap               | Used consistently as the level number label in Doom 2 and expansions based on it. Doom 1 level number label still uses ExMy. |
| You got... / Picked up... | Dapat...            | Used for pickup messages. These two message prefixes share the same translations to make the overall translation shorter.    |
| Ammo                      | Amunisi             | Amunisi is used instead of "Peluru" to not have it collide with the translation for the Bullet ammunition.                   |
| Shells                    | Peluru gotri        | "Peluru gotri" is used to distinguish shotgun ammunition from generic bullets. Abbreviated to `GTRI` on the status bar.      |
| Energy Cell               | Bateri              | A more natural representation of the Cell ammunition in Malay. Abbreviated to `BTRI` on the status bar.                      |
| Shotgun                   | Senapang Patah      | Super shotgun is translated to "Senapang Patah Super"                                                                        |
| Chaingun                  | Senapang Rantai     |                                                                                                                              |
| Plasma Rifle              | Rifel Plasma        |                                                                                                                              |
| Berserk                   | Penguat Otot Tangan | Lit. hand muscle strengthener. Describes the power-up's effect.                                                              |
| Supercharge               | Bebola Penyembuh    | Lit. healing orb. Descriptive localization based on its function.                                                            |
| Megasphere                | Bebola Penguat Diri | Lit. body-strengthening orb. Descriptive localization reflecting its function.                                               |

## Intermission Screen Terminology

Below are the terminologies used in the intermission screens and related places.

| English      | Malay        | Notes                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------ | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Kills        | Musuh        | Lit. enemy. Used instead of the direct translation "Bunuh" to not have it collide with the translation for "Frag".                                                                                                                                                                                                                                                                    |
| Items        | Item         |                                                                                                                                                                                                                                                                                                                                                                                       |
| Secret       | Rahsia       | Abbreviated to `RHSIA` in the co-op intermission screen.                                                                                                                                                                                                                                                                                                                              |
| Frag         | Bunuh        | Written in full on the status bar, abbreviated to `BNUH` in the co-op intermission screen.                                                                                                                                                                                                                                                                                            |
| Finished     | Selesai      |                                                                                                                                                                                                                                                                                                                                                                                       |
| Entering     | Memasuki     |                                                                                                                                                                                                                                                                                                                                                                                       |
| You Are Here | Kamu di Sini | Used in the intermission maps for Doom 1's Episode 1 through 3, as well as in Legacy of Rust's intermission maps.                                                                                                                                                                                                                                                                     |
| Victims      | Mangsa       | Used in the deathmatch intermission screen matrix.                                                                                                                                                                                                                                                                                                                                    |
| Killers      | Pembunuh     | Used in the deathmatch intermission screen matrix.                                                                                                                                                                                                                                                                                                                                    |
| Total        | Total        | Used in the deathmatch intermission screen matrix, as well as in the regular intermission screens in some ports.<br/>This string is not translated as `Jumlah` due to the graphic being long to the point of pushing the total time all the way to the right in some ports (such as Crispy Doom and Woof), while having high chance of the time overlapping the label in other ports. |

## Level Names Terminology

Level names are generally localized according to their meaning, tone, wordplay, and context rather than translated word-for-word.

Particular attention is given to titles containing jokes, idioms, Biblical references, archaic language, or unusual phrasing.

### Episode 4: Thy Flesh Consumed

The fourth episode of *The Ultimate Doom* contains level names inspired by Biblical passages. The original names use wording associated with the [King James Version](https://thekingsbible.com) (KJV), while the Malay localizations were developed with the corresponding passages in [Alkitab Versi Borneo](https://www.alkitabversiborneo.org) (AVB) as a reference.

The MalayDoom names are adaptations rather than direct quotations from either Bible translation. The passages below are included as references for the localization decisions.

| English                             | Malay                      | Reference Passage (English; KJV) | Reference Passage (Malay; AVB) |
| ----------------------------------- | -------------------------- | -------------------------------- | ------------------------------ |
| Thy Flesh Consumed (*episode name*) | Dagingmu Binasa            | Proverbs 5:11                    | Amsal 5:11                     |
| Hell Beneath                        | Alam Barzakh               | Proverbs 15:24                   | Amsal 15:24                    |
| Perfect Hatred                      | Sepenuh Kebencian          | Psalm 139:22                     | Mazmur 139:22                  |
| Sever The Wicked                    | Pengasingan Orang Durjana  | Matthew 13:49                    | Matius 13:49                   |
| Unruly Evil                         | Kejahatan Tidak Terkuasai  | James 3:8                        | Yakobus 1:5                    |
| They Will Repent                    | Mereka Akan Bertaubat      | Luke 16:30                       | Lukas 23:46                    |
| Against Thee Wickedly               | Terhadapmu dengan Kekejian | Psalm 139:20                     | Mazmur 139:20                  |
| And Hell Followed                   | Dan Neraka Mengekori       | Revelation 6:8                   | Wahyu 6:8                      |
| Unto the Cruel                      | Kepada yang Kejam          | Proverbs 5:9                     | Amsal 5:9                      |

### Wordplay, Jokes, and Unusual Phrasing

Some level names use puns, jokes, double meanings, idioms, or deliberately unusual wording.

Depending on the context, MalayDoom may preserve the original wordplay or tone, adapt it into a different Malay expression, or use a title that better reflects the level's setting or role in the game.

Examples include:

##### Doom II MAP07

**Original:** Dead Simple  
**MalayDoom:** Arena Pangkalan  
**Lit.:** Base Arena  
**Rationale:** The original title uses an idiom meaning “extremely easy,” with a fitting association with death. The localized title instead emphasizes the level's arena-like layout and setting.

##### Doom II MAP20

**Original:** Gotcha!  
**MalayDoom:** Gerbang Menuju Neraka  
**Rationale:** The original's colloquial expression was difficult to adapt naturally into Malay. The localized title instead emphasizes the level's role as a transition from the city levels to Hell.

#### Doom II MAP23

**Original:** Barrels o' Fun  
**MalayDoom:** Tong Keseronokan  
**Rationale:** A direct translation that retains the playful tone of the level name.

#### Plutonia MAP32

**Original:** Go 2 It  
**MalayDoom:** Maju-Maju Redah  
**Automap name:** Maju2 Redah  
**Lit.:** Keep Moving Forward and Charge Ahead  
**Rationale:** The localized title adapts the original's informal, action-oriented phrasing into Malay. The automap name uses the numeral “2” as a compact alternative spelling, echoing the original title's use of a numeral.

### Names Not Translated

Some level names are intentionally left untranslated.

This may apply to proper names, established fictional names, or terms where translating them would unnecessarily alter their identity or recognizability.

Examples include Doom's E3M8: **Dis**, TNT MAP26: **Ballistyx** and Plutonia MAP19: **NME**.

The same approach may also be used for monster names where the original name functions as a distinct fictional name. Examples include the **Ghoul**, **Banshee**, and **Vassago** from Legacy of Rust.

### Names with Retained Proper Names

Some of the level names have their proper name retained while the rest gets translated.

Examples include:

| Level     | MalayDoom Name | Notes                               |
| --------- | -------------- | ----------------------------------- |
| Doom E2M8 | Menara Babel   | *Babel* retained as a proper name.  |
| Doom E3M6 | Gunung Erebus  | *Erebus* retained as a proper name. |
| TNT MAP29 | Sungai Styx    | *Styx* retained as a proper name.   |

## Monster Names

The following are the localizations for all the monster names in Doom (not including Legacy of Rust, which are listed below)

| English           | Malay                    | Notes                                                                                                                                                            |
| ----------------- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Zombieman         | Zombi Askar              | Lit. soldier zombie.                                                                                                                                             |
| Shotgunner        | Zombi Bersenapang Patah  | Lit. zombie with shotgun.                                                                                                                                        |
| Chaingunner       | Zombi Bersenapang Rantai | Lit. zombie with chaingun.                                                                                                                                       |
| Imp               | Syaitan Kerdil           | Lit. dwarf demon.                                                                                                                                                |
| Demon (aka Pinky) | Syaitan Merah            | Lit. red demon. Referencing the pinkish-red look of the monster                                                                                                  |
| Spectre           | Syaitan Bayang           | Lit. shadow demon. Referencing the shadowy look of the fuzz effect                                                                                               |
| Lost Soul         | Jiwa yang Sesat          |                                                                                                                                                                  |
| Cacodemon         | Matagila                 | Referencing the one-eyed appearance of the monster.                                                                                                              |
| Baron of Hell     | Penguasa Neraka          | Also referenced in the following level names: TNT MAP25, Plutonia MAP06, No Rest for the Living MAP07.                                                           |
| Hell Knight       | Kesatria Neraka          |                                                                                                                                                                  |
| Mancubus          | Gergasi Buncit           | Lit. bloated giant. Referencing the more fatty appearance of the monster.                                                                                        |
| Arachnotron       | Lelabah Siber            | Lit. cyber spider.                                                                                                                                               |
| Pain Elemental    | Pembawa Sakit            | Lit. pain bringer.                                                                                                                                               |
| Revenant          | Mayat Hidup              |                                                                                                                                                                  |
| Arch-Vile         | Pembangkit Api Azab      | Lit. raiser of the fire of doom. Referencing both the fire attack and resurrection ability simultaneously. Yes the Azab part of the name is a Doom reference. :) |
| Spider Mastermind | Lelabah Pembawa Dalang   |                                                                                                                                                                  |
| Cyberdemon        | Syaitan Siber            |                                                                                                                                                                  |
| Icon of Sin       | Bapa Segala Dosa         | Same name as Doom 2's MAP30                                                                                                                                      |

## Legacy of Rust

*Legacy of Rust* introduces new weapons, ammunition types, monsters and related terminology that require additional localization decisions.

These names are generally localized according to their meaning and function while taking the original game's tone into account.

| English        | Malay            | Notes                                                                                          |
| -------------- | ---------------- | ---------------------------------------------------------------------------------------------- |
| Calamity Blade | Bilah Malapetaka | Lit. blade of calamity. Chosen to retain the weapon's dramatic tone.                           |
| Incinerator    | Penyembur Api    | Lit. flamethrower. Descriptive name based on its function.                                     |
| Fuel           | Minyak           | Lit. oil. Used for the new ammunition type. Abbreviated to `MNYK` on the status bar.           |
| Shocktrooper   | Zombi Plasma     | Lit. plasma zombie. Follows MalayDoom's established naming convention for zombie-type enemies. |
| Mindweaver     | Penganyam Minda  | Preserves the imagery of the original compound name.                                           |
| Tyrant         | Tiran            |                                                                                                |

## Cheat Code Messages

Below are cheat code messages that are not direct translation of the original message.

| Code(s)               | English                    | Malay                             | Notes                                     |
| --------------------- | -------------------------- | --------------------------------- | ----------------------------------------- |
| IDDQD                 | Degreelessness Mode ON/OFF | Mod Kebal BUKA/TUTUP              | Lit. Invulnerable mode.                   |
| IDKFA                 | Very Happy Ammo Added      | Senjata, Amunisi dan Kunci Diberi | Lit. Weapons, ammunitions and keys given. |
| IDFA                  | Ammo (no keys) Added       | Senjata dan Amunisi Diberi        | Lit. Weapon and ammunition given.         |
| IDCLIP<br/>IDSPISPOPD | No Clipping Mode ON/OFF    | Mod Tembus Tahap BUKA/TUTUP       | Lit. Pass through level mode.             |

## Translation Style

MalayDoom generally favors natural Malaysian Malay over rigid word-for-word translation.

When choosing between possible translations, the project may prioritize:

- Meaning and context

- Natural phrasing

- Tone and personality

- Humor and wordplay

- Dramatic or intentionally strange wording

- Consistency with established terminology

- Preservation of proper names where appropriate

Unusual wording in the original games is not automatically corrected. A phrase that sounds strange in English may be intentionally strange, and a literal translation is not always the best way to preserve that effect.

Where possible, MalayDoom aims to preserve the character and intent of the original text while making the result feel natural in Malaysian Malay.
