---
Type: Support
Cost: 1000
Restricted: false
Restrictions: 
Quality: "Each time you make this module active on your vehicle, choose a damage type: **air**, **bolt**, **earth**, **fire** or **ice**. Creatures aboard this vehicle are treated as being Resistant to the chosen damage type until this module remains active."
tags:
  - modules/rare
  - techno-fantasy-atlas
cssclasses:
  - Folder-3
  - alt-tint
---

> [!statblock|module] `=this.file.name` `=choice(this.Restricted = true, "(" + this.Restrictions + ")","")` _(`=this.Cost` z)_
> **`=this.Type` Module** ~ `=this.Quality`


