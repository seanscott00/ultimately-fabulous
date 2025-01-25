# Dataview

Made an effort to keep Dataview tables and lists in mind when styling, so hopefully stuff looks mostly consistent!

[Obsidian Dataview Documentation](https://blacksmithgu.github.io/obsidian-dataview/)




# Fantasy Statblocks Plugin

Custom CSS for statblocks from the Fantasy Statblocks plugin.

### Fabula Ultima Statblock


```statblock
layout: Fabula Ultima NPC
name: "Name of the Creature"
rank: rank #optional
level: X
species: "species"
description: "The creature's description, if presented here."

# Use "typicaltraits:" instead of "traits:" if the profile applies to an entire broad category of beings rather than a specific, one-of-a-kind entity.
traits: "Four traits. Use \"typical traits\" if the profile applies to an entire broad category of beings rather than a specific, one-of-a-kind entity."

DEX: X
INS: X
MIG: X
WLP: X

HP: 50
MP: X
DEF: X
MDEF: X
initiative: 10 #optional

# Affinities: physical, air, bolt, dark, earth, fire, ice, light, poison. All are optional. Only the listed affinities will appear on the sheet.
air: RS
earth: VU
poison: VU

# Use the attacks-m section for melee attacks and the attacks-r section for ranged -- these are only different in their icons. Both of these sections are technically optional, but the "Basic Attacks" heading will still appear, so please have at least one!
attacks-m:
  - name: "Melee attack"
    desc: "**[Check] + modifier (if any) ~ [damage formula] type** damage, followed by any special rule or effect."
attacks-r:
  - name: "Ranged attack"
    desc: "**[Check] + modifier (if any) ~ [damage formula] type** damage, followed by any special rule or effect."

# Spells -- this section is optional.
spells:
  - name: "Spell name ($ if offensive) ~ [Check] + modifier (if any) ~ Cost ~ Target ~ Duration."
    desc: "Effect."

# Skills are the "other actions" that appear with a gear symbol. This section is optional.
skills:
  - name: "Action name"
    desc: "See the rules for **writing an effect**."

# Rules -- this section is optional.
rules: 
  - name: "Rule name"
    desc: "See the rules for **writing an effect**."


```


### Stripped Statblock

> [!warning]
> This will return the styling of statblocks to the theme *no matter what statblock layout is used.* This will affect even the default statblock styles -- this may cause some unintended behavior.

```statblock
layout: Basic 5e Layout
creature: Adult Black Dragon
```




