---
Martial: true
Type: Armor
Cost: 150
DEF: "10"
MDEF: INS die
Initiative: -2
Quality: No Quality.
tags:
  - fabula-ultima
  - core-rulebook
  - armory/basic
cssclasses:
  - Folder-3
  - alt-tint
---

> [!statblock|armor] `=this.file.name` `=choice(this.Martial = true, "<span class='fu-mar'></span>","")` (`=this.Cost` z) _`=this.DEF` ~ `=this.MDEF` `=choice(this.Initiative != 0, "~ " + this.Initiative,"")`_
> **`=this.Type`** ~ `=this.Quality`