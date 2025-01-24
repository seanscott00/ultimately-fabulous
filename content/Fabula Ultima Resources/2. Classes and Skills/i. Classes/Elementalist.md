---
tags:
  - character-classes
  - core-rulebook
cssclasses:
  - Folder-2
  - alt-tint
---

[Free Benefits::MP +5 ▪ Ritualism]

## Elementalist Skills

### Cataclysm

![[Cataclysm|clean no-t]]

### Elemental Magic

![[Elemental Magic|clean no-t]]

### Magical Artillery

![[Magical Artillery|clean no-t]]

### Ritual Elementalism

![[Ritual Elementalism|clean no-t]]

### Spellblade

![[Spellblade|clean no-t]]

# Elementalist Spells

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
> FROM #spells and #elementalist 
> SORT file.name asc
> ```

# Heroic Skills

```dataview
LIST
FROM #skills/heroic AND [[]]
SORT file.name ASC
```

