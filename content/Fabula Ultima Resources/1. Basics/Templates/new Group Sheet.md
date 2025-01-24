---
cssclasses:
  - Folder-4
---

> [!infobox]
> ### &nbsp; Journal &nbsp;
> ```dataview
> TABLE WITHOUT ID file.link AS "Last 10 Entries"
> FROM #journal-entries 
> WHERE !contains(file.folder, "Templates")
> SORT date desc
> LIMIT 10
> ```


> [!callout|clean no-t flush]
> ### Group Notes and Clocks



Notes



> [!callout|clean no-t flush]
> ### Inventory Items
```dataview
TABLE WITHOUT ID file.link AS "Item",
IP AS "IP",
Effects AS "Effects"

FROM #inventory 
WHERE !contains(file.folder, "Templates")
SORT file.link asc
```


> [!callout|clean no-t flush]
> ### Party Overview
```dataview
TABLE WITHOUT ID "**" + file.link + " (lvl " + Level + ")**<br>*" + Identity + "*" AS "Character",
Theme + "<br>" + Origin + "<br>" + Quirk AS "Traits",
(MIG * 5 + Level + freeHP) + "HP" + " ~ " + "DEX d" + DEX + " ~ " + "INS d" + INS + " ~ " + "MIG d" + MIG + " ~ " + "WLP d" + WLP + " " + choice(contains(file.tags, "has-multi"), "⚔", "") + choice(contains(file.tags, "has-physical-damage"), "<span class='fu-phys'></span>", "") + choice(contains(file.tags, "has-air-damage"), "<span class='fu-air'></span>", "") + choice(contains(file.tags, "has-bolt-damage"), "<span class='fu-bolt'></span>", "") + choice(contains(file.tags, "has-dark-damage"), "<span class='fu-dark'></span>", "") + choice(contains(file.tags, "has-earth-damage"), "<span class='fu-earth'></span>", "") + choice(contains(file.tags, "has-fire-damage"), "<span class='fu-fire'></span>", "") + choice(contains(file.tags, "has-ice-damage"), "<span class='fu-ice'></span>", "") + choice(contains(file.tags, "has-light-damage"), "<span class='fu-light'></span>", "") + choice(contains(file.tags, "has-poison-damage"), "<span class='fu-psn'></span>", "") + "<br>" + Capabilities AS "Capabilities"
FROM #characters
WHERE !contains(file.folder, "Templates")
SORT level DESC, file.name ASC
```








