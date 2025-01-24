---
Martial: false
Type: Armor
Cost: 0
DEF: DEX die
MDEF: INS die
Initiative: 0
Quality: No Quality.
tags:
  - armory/rare
cssclasses:
  - Folder-3
  - alt-tint
---

> [!statblock|armor] `=this.file.name` `=choice(this.Martial = true, "<span class='fu-mar'></span>","")` (`=this.Cost` z) _`=this.DEF` ~ `=this.MDEF` `=choice(this.Initiative != 0, "~ " + this.Initiative,"")`_
> **`=this.Type`** ~ `=this.Quality`