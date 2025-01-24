---
tags:
  - character-classes
  - core-rulebook
cssclasses:
  - Folder-2
  - alt-tint
---

[Free Benefits::MP +5 ▪ Ritualism]

## Spiritist Skills

### Healing Power
![[Healing Power|clean no-t]]

### Ritual Spiritism
![[Ritual Spiritism|clean no-t]]

### Spiritual Magic
![[Spiritual Magic|clean no-t]]

### Support Magic
![[Support Magic|clean no-t]]

### Vismagus
![[Vismagus|clean no-t]]

# Spiritist Spells

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
> FROM #spells and #spiritist
> SORT file.name asc
> ```

### Heroic Skills

```dataview
LIST
FROM #skills/heroic AND [[]]
SORT file.name ASC
```
