---
cssclasses:
  - Folder-2
  - alt-tint
---

## Classes

> [!column|dataview 3 no-t] CLASSES
> ```dataview
> LIST WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + file.link + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","")
> FROM #character-classes AND !#template
> WHERE !contains(file.folder, "Templates")
> SORT file.name ASC
> ```

## Skills

> [!column|dataview 3 no-t] SKILLS
> ```dataview
> LIST WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + file.link + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","")
> FROM #skills and !#skills/heroic
> WHERE !contains(file.folder, "Templates")
> SORT file.name ASC
> ```

## Heroic Skills

> [!column|dataview 3 no-t] HEROIC SKILLS
> ```dataview
> LIST WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + file.link + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","")
> FROM #skills/heroic and !#skills/heroic/style
> WHERE !contains(file.folder, "Templates")
> SORT file.name ASC
> ```

## Spells

### Elementalist Spells

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
> FROM #spells and #elementalist 
> SORT file.name asc
> ```

### Entropist Spells

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
> FROM #spells and #entropist
> SORT file.name asc
> ```

### Spiritist Spells

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
> FROM #spells and #spiritist
> SORT file.name asc
> ```

### NPC Spells

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
> FROM #spells and #npc
> SORT file.name asc
> ```






