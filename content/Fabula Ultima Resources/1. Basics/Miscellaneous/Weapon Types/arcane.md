---
cssclasses:
  - Folder-1
  - alt-tint
---
#### Related Skills

> [!column|dataview flex no-t]
> ```dataview
> LIST WITHOUT ID choice(contains(file.tags, "core-rework"), "⋆","") + file.link + choice(contains(file.tags, "skills/heroic"), "⭐ ","")
> FROM #skills AND [[]]
> SORT file.name ASC
> ```

#### Related Items

> [!column|dataview flex no-t]
> ```dataview
> LIST WITHOUT ID choice(contains(file.tags, "core-rework"), "⋆","") + file.link + choice(contains(file.tags, "skills/heroic"), "⭐ ","")
> FROM #armory/rare AND [[]]
> SORT file.name ASC
> ```

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)" + "** " + Accuracy + " ~ " + Damage + " " + DamageType + "**<br>**" + Type + "** ~ " + Grip + " ~ " + Range + " ~ *" + Quality + "*" AS "Basic Arcane Weapons"
FROM #armory/basic
WHERE Type = "Arcane" AND !contains(file.folder, "Templates")
SORT Type, Cost, Name ASC
```

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + "**</span> (" + Cost + "z)" + "** " + Accuracy + " ~ " + Damage + " " + DamageType + "**<br>**" + Type + "** ~ " + Grip + " ~ " + Range + " ~ *" + Quality + "*" AS "Rare Arcane Weapons"
FROM #armory/rare
WHERE Type = "Arcane" AND !contains(file.folder, "Templates")
SORT Type, Cost, Name ASC
```

