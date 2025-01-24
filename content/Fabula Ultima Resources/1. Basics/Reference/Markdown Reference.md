---
cssclasses: []
---
## Headings

```
# heading
```

Headings go all the way to heading 6.

**Best Practices:** put a blank line before and after every heading!


> [!example|clean flush no-t]
> # Heading 1
> 
> ## Heading 2
> 
> ### Heading 3
 > 
> #### Heading 4
> 
> ##### Heading 5
> 
> ###### Heading 6
> 

## Paragraphs

Use a blank line to seperate one of more lines of text.

**Best Practices:** don't indent with spaces or tabs.

## Line Breaks

To create a line break or new line (`<br>`), end a line with two or more spaces ("trailing whitespace"), and then type return.

**Best Practices:** For compatibility, use trailing white space or the `<br>` HTML tag at the end of the line.

## Emphasis

`**bold text**`: **bold text**  

`__bold text__`: __bold text__  

`*italicized text*`: *italicized text*  

`_italicized text_`: _italicized text_  

`***bold and italicized text***`: ***bold and italicized text***  

`___bold and italicized text___`: ___bold and italicized text___  

`~~struck text~~`: ~~struck text~~  

`this is ==highlighted text==`: this is ==highlighted text==

**Best Practices:** if you need to bold or italicize within a word, use asterisks, not underscores.


## Blockquotes

Put a `>` in front of a paragraph to make a blockquote.

> Blockquote.

**Best Practices:** for compatibility, add a blank line before and after blockquotes.

## Lists

### Ordered Lists

To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one. To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab.

1. item 1
2. item 2
	1. item 2.1
	2. item 2.2
	3. item 2.3
		1. item 2.3.1
3. item 3
4. item 4

### Unordered Lists

To create an unordered list, add dashes (`-`), asterisks (`*`), or plus signs (`+`) in front of line items. Indent one or more items to create a nested list.

- item
- item
	- item
	- item
	- item
		- item
- item
- item

**Best Practices:** for compatibility, use the same delimiter across the whole list.

### Checkboxes

- [ ] Unchecked
- [x] Checked

## Code

To denote a word or phrase as code, enclose it in backticks (`` ` ``).

\`<code\>\`: `<code>`

To make a code block, indent the line by four spaces or a paragraph, or surround it in sets of three backticks (`` ``` ``).

```
<code>
```

(Note that if you have the **Dataview** plugin installed, `` `= `` will try to produce a dataview inline field.)

## Horizontal Rules

To create a horizontal rule, use three or more asterisks (`***`), dashes (`---`), or underscores (`___`) on a line by themselves.

```
***

---

_________________
```

The rendered output of all three looks identical:

***

**Best Practices:** for compatibility, put blank lines before and after horizontal rules.


## Wikilinks

`[[wikilink]]` places a [[link]]

`[[link#heading]]` links to a heading in a page [[To-Do Lists#Links]]

`[[link^block]]` links to a block

`![[link]]` embeds a link

`[[link|display text]]` changed the display text on the link

`[external link](https://bluecorvid.art/)` is an external link

`[[Fabula_Ultima_TTJRPG-core.pdf#page=70]]` links to a specific page in a pdf


## Tags

`#tag` makes a #tag

## Tables


| Table Header | Second Header |
| ------------ | ------------- |
| cell 1       | cell 2        |
| cell 3       | cell 4        |



## Callout Blocks

Callout blocks can have custom titles and are foldable. The title and body support markdown and can be nested. Using + makes the callout block foldable; using - makes it folded by default.

`> [!callout]`

>[!note]
>Unrecognized callout types will default to this type.

>[!column|3 clean] Examples
>
>> [!info]
>
>> [!Todo]
>
>> [!abstract]
>> Aliases: summary, tldr
>
>> [!tip]
>> Aliases: hint, important
>
>> [!success]
>> Aliases: check, done
>
>> [!question]
>> Aliases: help, faq
>
>> [!warning]
>> Aliases: caution, attention
>
>> [!failure]
>> Aliases: fail, missing
>
>> [!danger]
>
>> [!bug]
>
>> [!example]
>
>> [!quote]
>> Alias: cite