---
tags:
  - character-classes
  - high-fantasy-atlas
cssclasses:
  - Folder-2
  - alt-tint
---

[Free Benefits::MP + 5]
# Chanter Skills

### Magichant

![[Magichant|clean no-t]]

### Resonance

![[Resonance|clean no-t]]

### Siren's Song

![[Siren's Song|clean no-t]]

### Sound Barrier

![[Sound Barrier|clean no-t]]

### Vibrato

![[Vibrato|clean no-t]]

# Verses

## Frequencies

![[Frequencies|clean no-t]]

## Keys
```dataview
TABLE WITHOUT ID "**" + file.link + "**" AS "Key",
status AS "Status Effect",
attribute AS "Attribute",
recovery AS "Recovery"

FROM #magichant/keys 
SORT file.link asc
```


## Tones
```dataview
LIST WITHOUT ID "==**" + file.link + "**== ⋄ " + effect

FROM #magichant/tones
SORT file.link asc
```

# Heroic Skills
```dataview
LIST
FROM #skills/heroic AND [[]]
SORT file.name ASC
```
