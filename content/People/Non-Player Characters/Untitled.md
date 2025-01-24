---
Traits: four traits
Level: 5
Rank: Rank
Species: Species
Villain: false
VillainRank: Minor
UP: 5
DEX: 8
INS: 8
MIG: 8
WLP: 8
HP: 0
MP: 0
DEF: "8"
MDEF: "8"
Initiative: 0
Physical: none
Air: none
Bolt: none
Dark: none
Earth: none
Fire: none
Ice: none
Light: none
Poison: none
tags:
  - NPCs
cssclasses:
  - Folder-6
---

> [!infobox]
> 
> ![[avatar.png]]
> 
> ### `=choice(this.Villain = true, this.VillainRank + " Villain:", "")` `=this.Rank`
>
> ###### *`=this.Traits`*
> 
> |Level|`=this.Level`|Species|`=this.Species`|
> |:-|:-|:-|:-|
> | **DEX** | d`=this.DEX` | **DEF** | `=this.DEF` |
> | **INS** | d`=this.INS` | **M. DEF** | `=this.MDEF` |
> | **MIG** | d`=this.MIG` | **Init.** | `=this.Initiative` |
> | **WLP** | d`=this.WLP` |
>
> | HP | MP | `=choice(this.Villain = true, "UP", "")` |
> | :-: | :-: | :-:|
> | `=this.HP` ~ `=round(this.HP/2-0.5,0)` | `=this.MP` | `=choice(this.Villain = true, this.UP, "")`
> 
> | | | |
> | :-: | :-: | :-: |
> | `=choice(this.Physical = "none", "<span class='fu-phys-s'></span>", "<span class='fu-phys'></span> " + this.Physical)` | `=choice(this.Air = "none", "<span class='fu-air-s'></span>", "<span class='fu-air'></span> " + this.Air)` | `=choice(this.Bolt = "none", "<span class='fu-bolt-s'></span>", "<span class='fu-bolt'></span> " + this.Bolt)` |
> | `=choice(this.Dark = "none", "<span class='fu-dark-s'></span>", "<span class='fu-dark'></span> " + this.Dark)` | `=choice(this.Earth = "none", "<span class='fu-earth-s'></span>", "<span class='fu-earth'></span> " + this.Earth)` | `=choice(this.Fire = "none", "<span class='fu-fire-s'></span>", "<span class='fu-fire'></span> " + this.Fire)` |
> | `=choice(this.Ice = "none", "<span class='fu-ice-s'></span>", "<span class='fu-ice'></span> " + this.Ice)` | `=choice(this.Light = "none", "<span class='fu-light-s'></span>", "<span class='fu-light'></span> " + this.Light)` | `=choice(this.Poison = "none", "<span class='fu-psn-s'></span>", "<span class='fu-psn'></span> " + this.Poison)` |
> 

> [!info|clean no-t flush]
> ## Description


Description


> [!list|melee clean no-title flush]
> ### Basic Attacks
> 
> - **Melee Attack ~ [Check] + modifier (if any) ~ [damage formula] type** damage, followed by any special rule or effect.

> [!list|ranged clean no-title flush]
> - **Ranged Attack ~ [Check] + modifier (if any) ~ [damage formula] type** damage, followed by any special rule or effect.

> [!list|spells clean no-title flush]
> ### Spells
> - **Spell name (<span class="fu-off"></span> if offensive) ~ [Check] + modifier (if any) ~ Cost ~ Target ~ Duration.**  
Effect.

> [!list|skills clean no-title flush]
> ### Other Actions
> - **Action name** ~ See the rules for **writing an effect**.

> [!list|rules clean no-title flush]
> ### Special Rules
> - **Rule name** ~ See the rules for **writing an effect**.

> [!info|clean no-t flush]
> ## Items
>> [!statblock]- Rewards
>> Items and zenit
>> 
>
>> [!statblock|treasure]- Soul Treasure
>> Item
