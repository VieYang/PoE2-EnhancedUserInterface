## CHANGELOG
### 0.6.1-beta.2
- Changed the color of reputation gains and losses to a slightly darker hue.
### 0.6.1-beta.1
- Removed duplicated text sections from the Penetration entry (cyclopedia.stringtable).
- Removed a unnecessary keyword stylization from entry ID `435` (abilities.stringtable).
- Added missing keywords to entries `4416`, `4419`, `4420` and `4422` (abilities.stringtable).

### 0.6.0
**Abilities.stringtable**:\
- Removed a duplicated `line-height` tag in ID 564 (abilities.stringtable).
- Added the "Penetrate" keyword to 32 new entries (abilities.stringtable).
- Added the keyword "Armor Rating" to 14 new entries (abilities.stringtable).
- Removed ID incorrectly applied text stylization to ID 607, 631, 643, 811, 1573, 1962, 1964, 1967, 1968, 2271, 2896, 2898, 2900 and 2902 (abilities.stringtable).
- Added missing keywords to ID's 614, 831, 925, 2039, 2663, 2732, 3923, 4092, 4166 and 4774 (abilities.stringtable).
- Might inspiration Energized should now have the correct color code (abilities.stringtable).
- Fixed broken links to glossary entry `Terrified` (abilities.stringtable).
**Cyclopedia.stringtable**:\
- Added missing `line-height` tag in ID `679 (cyclopedia.stringtable).
- Added support for the keywords `Armor Rating` and `Penetrate (cyclopedia.stringtable).
**Gui.stringtable**:\
- Added a lot of missing entries (gui.stringtable).
**Items.stringtable**:\
- Added a few missing font tags to multiple entries (items.stringtable).
**Statuseffects.stringtable**:\
- Added missing `line-height` tags (statuseffects.stringtable).
- Fixed a few incorrectly applied font stylizations (statuseffects.stringtable).

### 0.5.2
- Updated the mod for game build `1.2.0.0008`.
### 0.5.1
- Added missing keywords to Entry `240` and `1470`.
- Added missing cyclopedia link and icon to the keyword "Armor Rating" in `statuseffects.stringtable`.
- Removed an incorrectly applied keyword to ID `603` in `abilities.stringtable`.
- Added missing line-height tags to ID's `240`, `1470` and `3677` in `abilities.stringtable`.
### 0.5
- Changed the font of rank 1 afflictions and inspirations to something more distinctive (I picked `EspinosaNova-Regular SDF` instead of `EBGaramond-Regular SDF`) - not final, probably.
- The keywords `Might` and `Tenacious` now have the correct color code (from `#f7b733` to `#ff4800`).
- Fixed a wrongly (?) applied icon in entry #1270 (`abilities.stringtable`):
> Summons three missiles that each ~~`&lt;link="glossary://GlossaryEntry_Piercing"&gt;&lt;b&gt;`~~ pierce ~~`&lt;/b&gt;&lt;space=0.7em&gt;&lt;sprite="Inline" name="cs_pierce" tint=1&gt;&lt;/link&gt;`~~ through the target and then leap to additional targets.

- Updated `statuseffects.stringtable` to match the font stylizations in the other `.stringtable-files`.
- All icons and ranks now have the same distance between the keyword and the icon (`0.7em`) and the icon and the rank indicator (`0.3em`). Probably needs further adjustments for each attribute to look "just right".
- Attribute titles in entries `94`, `96`, `98`, `100`, `102`, `106`, `108`, `110`, `116`, `118`, `120`, `122`, `124`, `322`, `533`, `679`, `681`, `683`, `713`, `715`, `717`, `719`, `721`, `723`, `725`, `727`, `729`, `731`, `733`, `735`, `737`, `739`, `741`, `743`, `745`, `747` in `cyclopedia.stringtable` should now all have the same font size and placement.
- Added missing `<FemaleText />` and `</Entry>` tags to ID `9`.\

**Side note(s):**
- Added a lot of improvements to the macros I'm using which should result in less buggy texts as well as making it easier to adapt to future patches to the main game.
- I'm using this RegEx to remove all text except the Entry ID's: `[\S\s]+?<ID>(\d+?)<\/ID>`\
  It's a neat little RegEx to use if you want to get a list of all ID's in a `.stringtable` file.

***

### 0.4
- On par with de_patch

***

### 0.3.2-04
- Added a better description to the "Death Runes" status effect. (abilities.stringtable ID #3677) /Spherikal

### 0.3.2-03
- Fixed a issue where status effects and item descriptions swapped places.

### 0.3.2-01
- Fixed a few incorrect keyword stylizations.
- Might inspirations should now use the new icon and rank syntax.
- Slightly increased the distance between Constitution icons and ranks
- Added some missing status effect Entries.
- Fixed a issue with cyclopedia entries.

### 0.3.2
- Huge changes to how Affliction and Inspiration icons are displayed. No need for sub/sup tags or similar anymore.
- Line heights should no longer be affected by icon size or text palcement (the <voffset> tag for example).


### 0.3.1
- Added subscript for all negative afflictions.
- Changed the color of Perception to a slightly lighter hue for easier reading.
- Made the damage type text bold and set a fixed width between the damage keyword and it's corresponding icon.
- Changed the distance between the Dexterity icon and it's rank indicator.
- Added color for reputation gain in gui.stringtable
- Added cyclopedia entries for all damage types.
- Added icon to defensive stats.
- Fixed some Resolve keywords getting the wrong color and icon.
- No afflictions or inspirations should no longer have a bold text effect (didn't look quite right).
- Changed the distance between Shock text and icon.
