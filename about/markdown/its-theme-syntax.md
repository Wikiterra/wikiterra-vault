# ITS Theme (markdown syntax)

### Alternate Color Schemes
- [x] Schools Days
- [x] TTRPG: Pathfinder

```json
{
  "ITS@@accent-color": false,
  "ITS@@slrvb-b": false,
  "ITS@@its-d": false,
  "ITS@@notion": false,
  "ITS@@mini": false,
  "ITS@@slrvb-g": false,
  "ITS@@s-d": true,
  "ITS@@t-d": false,
  "ITS@@nord": false,
  "ITS@@drwn": false,
  "ITS@@select": "pathfinder"
}
```

---

## Callouts

### Asides
```markdown
> [!aside|clean right]
> Removes styling from aside

> [!aside|tufte]+ 
> Tufte styled aside callout

> [!aside|tufte title]
> Show callout title for asides
```

### Captions
```markdown
> [!caption|left] Floats to the left
> ![[Image.png]]
> Caption text here

> [!caption|right] Floats to the right
> ![[Image.png]]
> Caption text here
```

### Cards
```markdown
> [!cards|4]
> **[[Link]]**
> ![Image link|sban htiny ctr](https://images.unsplash.com/photo-1574375927938-d5a98e8ffe85?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&cs=srgb&w=1200)
> 
> **[[Link]]**
> ![[Image Link.png|sban htiny ctr]]
> 
> **[[Link]]**
> ![Image link|sban htiny ctr](https://images.unsplash.com/photo-1574375927938-d5a98e8ffe85?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&cs=srgb&w=1200)
> 
> **[[Link]]**
> ![[Image Link.png|sban htiny ctr]]
```

### Checks
```markdown
> [!checks]
> - **GROUP**
> 	- Next to checkboxes
> 	- [ ] %% %%
> 	- [ ] %% %%
> 	- [ ] %% %%
> 	- [ ] %% %%
> 	- [ ] %% %%
> - **New Row**
> 	- Description
> 	- [ ] %% %%
> 	- [ ] %% %%
> 	- [x] %% %%
> 	- [x] %% %%
> 	- [x] %% %%
> - 
> 	- Empty root bullet is necessary to group bullets together
> 	- [x] %% %%
> 	- [x] %% %%
> 	- [x] %% %%
> 	- [ ] %% %%
> 	- [ ] %% %%
```

### Colors
```markdown
> [!recite|color-blue]

> [!recite|background-blue]

> [!recite|background-color-blue]
```

### Columns
```markdown
> [!column]
>> [!info] Column 1
>> - Use another callout for columns
>
>> [!note] Column 2
>> Need that singular blockquote `>` as separation between columns
```

### Grid
```markdown
> [!grid]
> ![[column-1.jpg]]
> ![[column-3.jpg]]
>
> ![[column-2.jpg]]

> [!grid|masonry]
> ![External Image 1](https://www.dmuth.org/wp-content/uploads/2021/03/obsidian-logo.png)
> ![External Image 2](https://www.dmuth.org/wp-content/uploads/2021/03/obsidian-logo.png)
> 
> ![External Image 3 on New Row](https://www.dmuth.org/wp-content/uploads/2021/03/obsidian-logo.png)
```

### Infoboxes
```markdown
> [!infobox|left wikipedia]+
> # Heading
> ![[Image.png]]
> ###### Heading 6
> | Table Header |  Table Header |
> | ---- | --- |
> | Test | Testing |
> | Test | Testing |
> 
> # Heading 1
> - Bullet list
> 	- Testing
> 	- Testing
> - Testing
```

### Kanban
```markdown
> [!kanban]+
> - [[Link|Lane 1 Title]]
> 	- ![[Image.png]]
> 	- [[Link|Card]]
> - [[Link|Lane 2 Title]]
> 	![[Image without background card styling.png]]
> 	- [[Link|Card]]
> - Text
> 	- [ ] Text
```

### Kith
```markdown
> [!kith|relationship] **Character Name** _Subtitle/Brief Relationship Description_
```

### Metadata
> [!Metadata]
> **Bold Text** Regular Text  
> **Dataview Inline Field**:: Value

### Quote
```markdown
> [!quote|author] Quote Author Here
> Blockquote text here

> [!quote|mark] Author
> Quote with Mark

> [!quote] Quote Author Here <br>New Line stuff here
> Blockquote text here
```

### Starblocks
```markdown
> [!statblocks]
> ![Char Image|cover right circle htiny wtiny lp](github-logo.png)
> 
> # Name
> > Description
> *Basics*
> *Basics*
> 
> ---
| HP | AC | Initiative |
|:---:|:---:|:---:|
| | | |
>
| STR | DEX | CON | INT | WIS | CHA |  |
|:---:|:---:|:---:|:---:|:---:|:---:|:--- |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  | **Mod** |
|  |  |  |  |  |  | **Sav** |
> 
|  |  |
| ---:|:--- |
| **Speed** |  |
| **Passive Perception (WIS)** |  |
| **Proficiency Bonus** |  |
| **Darkvision** |  |
>
> ---
>> [!checks|no-t] 
>> - **Death Saves**
>>	- ❌
>>	- [ ] 
>>	- [ ] 
>>	- [ ] 
>>	- ✔
>>	- [ ] 
>>	- [ ] 
>>	- [ ] 
>
> ###### Traits
| | |
| --- | --- |
| **Class** | |
| **.** | |
| **Racial Traits** | |
| **Feats** | |
```

### Timeline
```markdown
> [!timeline|t-l] **Title** _Subtitle_
> Left aligned timeline piece

> [!timeline|t-r t-4] **Title** *Subtitle*
> Right aligned timeline piece

> [!timeline|t-r t-10] **Title** *Subtitle*
> Spaced timeline piece
```

## References

- [ITS Theme Documentation](https://publish.obsidian.md/slrvb-docs/ITS+Theme/ITS+Theme)
- [Callout+Adjustments - ITS Theme Documentation](https://publish.obsidian.md/slrvb-docs/ITS+Theme/Callout+Adjustments)

---

## ITS Theme Settings
### Alternate Color Schemes
- [x] Schools Days
- [x] TTRPG: Pathfinder

```json
{
  "ITS@@accent-color": false,
  "ITS@@slrvb-b": false,
  "ITS@@its-d": false,
  "ITS@@notion": false,
  "ITS@@mini": false,
  "ITS@@slrvb-g": false,
  "ITS@@s-d": true,
  "ITS@@t-d": false,
  "ITS@@nord": false,
  "ITS@@drwn": false,
  "ITS@@select": "pathfinder"
}
```