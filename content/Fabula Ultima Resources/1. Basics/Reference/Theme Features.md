---
cssclasses: []
---
## Style Settings

#### Remove H1 Background

This might look nicer if you have inline titles turned off.

#### Increased Link Visibility

Returns link underlines -- might be useful if you're using a darker accent color that makes links less visible.

#### Alternative Tints

Reverses the hue shift used on certain elements. You can apply this to individual notes by adding the `cssclasses: alt-tint` property to it.

#### Fonts

A selection of settings to let you change the fonts used in the vault without disrupting the inline icons like ~ and ].

If you change the vault fonts in Obsidian's main Appearance menu, add the font *Fabula Inline* to the top of your fonts list.

#### Folder Colors

This setting will allow you to apply colors to the first six folders in the file viewer. They can also be applied to individual notes by giving those notes the corresponding CSS classes in their frontmatter.

<table>
	<tr>
		<th>Folder</th><th>CSS Class</th><th>Default Color</th><th>Current Color</tr>
	</th>
	<tr>
		<td>Folder 1</td>
		<td><code>Folder-1</code></td>
		<td style="background:#E57185;">#E57185</td>
		<td style="background:var(--sg-folder1-color);"></td>
	</tr>
	<tr>
		<td>Folder 2</td>
		<td><code>Folder-2</code></td>
		<td style="background:#E8D571;">#E8D571</td>
		<td style="background:var(--sg-folder2-color);"></td>
	</tr>
	<tr>
		<td>Folder 3</td>
		<td><code>Folder-3</code></td>
		<td style="background:#8DBC5D;">#8DBC5D</td>
		<td style="background:var(--sg-folder3-color);"></td>
	</tr>
	<tr>
		<td>Folder 4</td>
		<td><code>Folder-4</code></td>
		<td style="background:#4C9FAE;">#4C9FAE</td>
		<td style="background:var(--sg-folder4-color);"></td>
	</tr>
	<tr>
		<td>Folder 5</td>
		<td><code>Folder-5</code></td>
		<td style="background:#3962D4;">#3962D4</td>
		<td style="background:var(--sg-folder5-color);"></td>
	</tr>
	<tr>
		<td>Folder 6</td>
		<td><code>Folder-6</code></td>
		<td style="background:#7E3B97;">#7E3B97</td>
		<td style="background:var(--sg-folder6-color);"></td>
	</tr>
</table>

##### Accent Color Palette

<table style="border:0px;">
	<tr style="border:0px;">
		<td style="background:hsl(var(--sg-tint-darkest));color:var(--background-primary);">Tint Darkest</td>
		<td style="background:hsl(var(--sg-tint-darker));color:var(--background-primary);">Tint Darker</td>
		<td style="background:hsl(var(--sg-tint-dark));color:var(--background-primary);">Tint Dark</td>
		<td style="background:var(--text-accent);">Accent Color</td>
		<td style="background:hsl(var(--sg-tint-bright));">Tint Bright</td>
		<td style="background:hsl(var(--sg-tint-brighter));">Tint Brighter</td>
		<td style="background:hsl(var(--sg-tint-brightest));">Tint Brightest</td>
	</tr>
	<tr style="border:0px;">
		<td style="background:hsl(var(--sg-accent-darkest));color:var(--background-primary);">Accent Darkest</td>
		<td style="background:hsl(var(--sg-accent-darker));color:var(--background-primary);">Accent Darker</td>
		<td style="background:hsl(var(--sg-accent-dark));color:var(--background-primary);">Accent Dark</td>
		<td style="background:var(--text-accent);">Accent Color</td>
		<td style="background:hsl(var(--sg-accent-bright));">Accent Bright</td>
		<td style="background:hsl(var(--sg-accent-brighter));">Accent Brighter</td>
		<td style="background:hsl(var(--sg-accent-brightest));">Accent Brightest</td>
	</tr>
	<tr style="border:0px;">
		<td style="background:hsl(var(--sg-alt-darkest));color:var(--background-primary);">Alt Darkest</td>
		<td style="background:hsl(var(--sg-alt-darker));color:var(--background-primary);">Alt Darker</td>
		<td style="background:hsl(var(--sg-alt-dark));color:var(--background-primary);">Alt Dark</td>
		<td style="background:var(--text-accent);">Accent Color</td>
		<td style="background:hsl(var(--sg-alt-bright));">Alt Bright</td>
		<td style="background:hsl(var(--sg-alt-brighter));">Alt Brighter</td>
		<td style="background:hsl(var(--sg-alt-brightest));">Alt Brightest</td>
	</tr>
</table>

## Icons

From the *Fabula Ultima Icons Regular* font. These can be inserted with some HTML.

| Icon                           | Code                             | Icon                             | Code                               |
| ------------------------------ | -------------------------------- | -------------------------------- | ---------------------------------- |
| <span class='fu-phys'></span>  | `<span class='fu-phys'></span>`  | <span class='fu-phys-s'></span>  | `<span class='fu-phys-s'></span>`  |
| <span class='fu-air'></span>   | `<span class='fu-air'></span>`   | <span class='fu-air-s'></span>   | `<span class='fu-air-s'></span>`   |
| <span class='fu-bolt'></span>  | `<span class='fu-bolt'></span>`  | <span class='fu-bolt-s'></span>  | `<span class='fu-bolt-s'></span>`  |
| <span class='fu-dark'></span>  | `<span class='fu-dark'></span>`  | <span class='fu-dark-s'></span>  | `<span class='fu-dark-s'></span>`  |
| <span class='fu-earth'></span> | `<span class='fu-earth'></span>` | <span class='fu-earth-s'></span> | `<span class='fu-earth-s'></span>` |
| <span class='fu-fire'></span>  | `<span class='fu-fire'></span>`  | <span class='fu-fire-s'></span>  | `<span class='fu-fire-s'></span>`  |
| <span class='fu-ice'></span>   | `<span class='fu-ice'></span>`   | <span class='fu-ice-s'></span>   | `<span class='fu-ice-s'></span>`   |
| <span class='fu-light'></span> | `<span class='fu-light'></span>` | <span class='fu-light-s'></span> | `<span class='fu-light-s'></span>` |
| <span class='fu-psn'></span>   | `<span class='fu-psn'></span>`   | <span class='fu-psn-s'></span>   | `<span class='fu-psn-s'></span>`   |
| <span class='fu-off'></span>   | `<span class='fu-off'></span>`   | <span class='fu-mar'></span>     | `<span class='fu-mar'></span>`     |






## Custom Callouts


### Callout Adjustments

`> [!callout|adjustments]`

| Adjustment code | Adjustment alias |                                                                                                               |
| :-------------: | :--------------: | :------------------------------------------------------------------------------------------------------------ |
|    `accent`     |                  | uses the page accent color for the callout background. unfinished.                                            |
|     `clean`     |                  | removes most styling; also works on embeds                                                                    |
|     `flush`     |                  | pushes contents up against the left side of the page -- made for containing content next to floating elements |
|     `left`      |      `p+l`       | makes the callout float to the left                                                                           |
|    `no-icon`    |      `no-i`      | removes icon                                                                                                  |
|   `no-title`    |      `no-t`      | removes the title; also works on embeds                                                                       |
|     `right`     |      `p+r`       | makes the callout float to the right                                                                          |
|   `subtitle`    |      `subt`      | italic text in the title will become a subtitle                                                               |
|    `no-link`    |      `nlk`       | for embeds; no link icon     |





### Statblock Calloutss
Icons from Game-icons.net.

`> [!statblock|(type)]`

> [!statblock] Statblock _offset subtitle_
> I'm just about happy with how these look, I think.

> [!column|3 clean] Examples
>> [!statblock|arcane] Arcane
>> Weapon
>
>> [!statblock|bow] Bow
>> Weapon
>
>> [!statblock|brawling] Brawling
>> Weapon
>
>> [!statblock|dagger] Dagger
>> Weapon
>
>> [!statblock|firearm] Firearm
>> Weapon
>
>> [!statblock|flail] Flail
>> Weapon
>
>> [!statblock|heavy] Heavy
>> Weapon
>
>> [!statblock|spear] Spear
>> Weapon
>
>> [!statblock|sword] Sword
>> Weapon
>
>> [!statblock|thrown] Thrown
>> Weapon
>
>> [!statblock|armor] Armor
>> Armor
>
>> [!statblock|shield] Shield
>> Shield
>
>> [!statblock|accessory] Accessory
>> Accessory
>
>> [!statblock|module] Module
>> Module
>
>> [!statblock|creature] Creature
>> Creature
>
>> [!statblock|person] Person
>> Person
>
>> [!statblock|place] Place
>> Place
>
>> [!statblock|treasure] Treasure
>> Treasure

### List Callouts

`> [!list|inline]`

> [!list|inline]
> - [ ] task
> - [ ] list
> - [ ] items
> - [ ] appear
> - [ ] inline
> - [ ] instead
> - [ ] of
> - [ ] on
> - [ ] their
> - [ ] own
> - [ ] lines

`> [!list|melee/ranged/spells/skills/rules]`

> [!list|melee] Melee Attacks
> - Attack
> - Attack
> - Attack


> [!list|ranged no-title] Ranged Attacks
> - Attack
> - Attack

> [!list|spells] Spells
> - Spell
> - Spell

> [!list|skills] Skills
> - Skill
> - Skill

> [!list|rules] Rules
> - Rule
> - Rule

> [!bug]
> I haven't gotten these to work in live edit yet...
















### Column Calloutss

```
> [!column]
>> [!info] Column 1
>> - Use another callout for columns
>
>> [!note] Column 2
>> Need that singular blockquote `>` as separation between columns
```

> [!column]
>> [!info] Column 1
>> - Use another callout for columns
>
>> [!note] Column 2
>> Need that singular blockquote `>` as separation between columns

> [!info] Adjustments for Column Callouts
> `(number of columns)`  
> `flex`  
> `list`  



### Image Grid Callouts

`> [!grid|(masonry)]` (use masonry for externally-linked images)

> [!grid]
> ![[avatar.png|avatar.png]]
> ![[avatar.png|avatar.png]]
> ![[avatar.png|avatar.png]]
>
> ![[avatar.png|avatar.png]]
> ![[avatar.png|avatar.png]]



### Bond Callouts

`> [!bond|type] **Character Name** _subtitle_`

This is the same as ITS "kith" callouts. I mean to restyle them.

>[!bond|relationship] **Character Name** _Subtitle/Description_
>Relationship Types
>- family
>- friend
>- romantic
>- antagonist

> [!column]
>>[!bond|family] Family
>
>> [!bond|friend] Friend
>
>>[!bond|romantic] Romantic
>
>>[!bond|antagonist] Antagonist


### Caption Callouts

```
> [!caption]
> (image)
> (caption text)
```


> [!caption] A caption for an image?
> ![[avatar.png|avatar.png]]
> Caption text here.


### Infobox Callouts

`> [!infobox]`

> [!infobox]- title?
> # INFOBOX
> ![[avatar.png|avatar.png]]
> ###### Customizations
> | code | does what? |
> | ---- | ---- |
> | + | collapsible |
> | - | collapsed by default |
> | left | puts it on the left |
> |show-title| (s-t) shows the title|

These float on top of other content, which clashes badly with the formatting of some themes. Using a `clean` callout to contain content that will be pushed to the side will prevent a lot of weirdness.





