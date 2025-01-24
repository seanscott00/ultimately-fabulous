---
cssclasses:
  - Folder-3
  - alt-tint
---
## Basic Equipment

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)" + "** " + Accuracy + " ~ " + Damage + " " + DamageType + "**<br>**" + Type + "** ~ " + Grip + " ~ " + Range + " ~ *" + Quality + "*" AS "Weapons"
FROM #armory/basic
WHERE Type != "Armor" AND Type != "Shield" AND !contains(file.folder, "Templates")
SORT Type, Cost, Name ASC
```

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)** " + DEF + " ~ " + MDEF + choice(contains(file.fields, Initiative), "", " ~ " + Initiative + " init.") + "**<br>" + "**" + Type + "** ~ *" + Quality + "*" AS "Armor"
FROM #armory/basic
WHERE Type = "Armor" AND !contains(file.folder, "Templates")
SORT Cost, Name ASC
```

```dataview
TABLE WITHOUT IDchoice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)** " + DEF + " ~ " + MDEF + choice(contains(file.fields, Initiative), "", " ~ " + Initiative + " init.") + "**<br>" + "**" + Type + "** ~ *" + Quality + "*" AS "Shields"
FROM #armory/basic
WHERE Type = "Shield" AND !contains(file.folder, "Templates")
SORT Cost, Name ASC
```



## Rare Equipment


```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + "**</span> (" + Cost + "z)" + "** " + Accuracy + " ~ " + Damage + " " + DamageType + "**<br>**" + Type + "** ~ " + Grip + " ~ " + Range + " ~ *" + Quality + "*" AS "Weapons"
FROM #armory/rare
WHERE Type != "Armor" AND Type != "Shield" AND Type != "Accessory" AND !contains(file.folder, "Templates")
SORT Type, Cost, Name ASC
```

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)** " + DEF + " ~ " + MDEF + choice(contains(file.fields, Initiative), "", " ~ " + Initiative + " init.") + "**<br>" + "**" + Type + "** ~ *" + Quality + "*" AS "Armor"
FROM #armory/rare
WHERE Type = "Armor" AND !contains(file.folder, "Templates")
SORT Cost, Name ASC
```

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)** " + DEF + " ~ " + MDEF + choice(contains(file.fields, Initiative), "", " ~ " + Initiative + " init.") + "**<br>" + "**" + Type + "** ~ *" + Quality + "*" AS "Shields"
FROM #armory/rare
WHERE Type = "Shield" AND !contains(file.folder, "Templates")
SORT Cost, Name ASC
```

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)<br>" + "**" + Type + "** ~ *" + Quality + "*" AS "Accessories"
FROM #armory/rare
WHERE Type = "Accessory" AND !contains(file.folder, "Templates")
SORT Cost, Name ASC
```

# Rare Item Qualities

```dataview
TABLE WITHOUT ID "**" + file.link + "**" AS "Item Quality",
choice(contains(file.tags, "weapon"), "✔", "❌") AS "🗡",
choice(contains(file.tags, "armor"), "✔", "❌") AS "🥋",
choice(contains(file.tags, "accessory"), "✔", "❌") AS "💍",
Cost AS "Cost",
Description as "Description"

FROM #qualities
WHERE !contains(file.folder, "Templates")
SORT Cost, Name asc
```

