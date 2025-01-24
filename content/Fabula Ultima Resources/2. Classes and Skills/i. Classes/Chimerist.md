---
tags:
  - character-classes
  - core-rulebook
cssclasses:
  - Folder-2
  - alt-tint
---

[Free Benefits::MP +5 ▪ Ritualism]
## Chimerist Skills

### Consume

![[Consume|clean no-t]]

### Feral Speech

![[Feral Speech|clean no-t]]

### Pathogenesis

![[Pathogenesis|clean no-t]]

### Ritual Chimerism

![[Ritual Chimerism|clean no-t]]

### Spell Mimic

![[Spell Mimic|clean no-t]]

## NPC Spells

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
> FROM #spells and #npc
> SORT file.name asc
> ```

# Heroic Skills

```dataview
LIST
FROM #skills/heroic AND [[]]
SORT file.name ASC
```
