# Headings (1) `#`

## Heading 2 `##`

### Heading 3 `###`

#### Heading 4 `####`

##### Heading 5 `#####`

###### Heading 6 `######`

body text

# Horizontal Line `---`

This is the horizontal line

---

# Line Breaks (Double rule) or `<br>`


In the editor:
This line is above.
This line is below.
But these all output on the same line.


## Solution 1:

Make sure that 

Each separated line/element

Is 'Double spaced'

## Solution 2: 

Use `<br>`<br>
To get things <br>
On the next line, but closer

# Text Formatting


## Bolding: `**text**` or `__text__`

**Bolded text** done using `**Bolded Text**`

__Bolded text__ done using `__Bolded Text__`

## Italicising: `*text*` or `_text_`

*Italicised text* done using `*Italicised text*`

_Italicised text_ done using `_Italicised text_`

## Strikethrough: `~~text~~`

~~strikethrough text~~ done using `~~strikethrough text~~`

## Change font color: `<font color = color>text</font>`

<font color = green>Green Light</font>, <font color = red>Red Light</font>

<font color = #f0ff18>you can use hexcodes too</font>

## Superscript `<sup>text</sup>` and Subscript `<sub>text</sub>`

A = B<sub>1</sub>X<sub>1</sub> + B<sub>2</sub>X<sub>2</sub><sup>2</sup> + C

## Hyperlinking

### Internally, within this markdown/ipynb headers
- E.g. [Horizontal Line](#horizontal-line) section
    - `[Text](#formatted-header-name)`
    - E.g. `[Headings](#headings-1)` gets you [Headings](#headings-1)
    - Good for making a directory / table of contents

### To external site
- E.g. [My Spotify Channel](https://open.spotify.com/artist/6UgKxnAe4kVYqLJPcfTboF?si=2HJUNAHmQuC0Y-qnn-WvBw)
    - `[Text](https://www.website.com/)`
    - E.g. `[My Youtube Channel](https://www.youtube.com/@choonxyong/)` gets you [My Youtube Channel](https://www.youtube.com/@choonxyong/)

# Listing


## Ordered listing `123`

>note that 123 works but abc doesnt...

1. text
    1. text
    2. text
2. text
    1. text
    2. text
        1. text
3. text
    1. text
    2. text

## Unordered listing `- `

- text
    - text
    - text
- text
    - text
    - text
        - text
- text
    - text
    - text



## Task Listing `- [ ]` / `- [x]`
- [x] Task 1
- [ ] Task 2
- [ ] Task 3

# Images


> Recommendation: use publicly available image(s) that will readily load in. 

> Otherwise, user's system must also have the image(s) downloaded locally somewhere


## Public Images `<img src = "https://link_to_image/">`

> Arguments to call in \<img\>
>
> ```html
> <img 
>    src = 'https://link_to_image/' 
>    alt = 'alternate text if image cant load' 
>    width="number_value"   
>    height ="number_value"
>    >
> ```
>>>

> You can also embed link in image through:
> ```html
> <a href ="https://website"><img src = "https://link_to_image"></a>
> ```

> Notice How images fill into to the right until there's no more space, then goes down ... just like text

> Use `<br>` to force vertical stacking of images

Examples:

<a href="https://open.spotify.com/track/2Th0Xb1xVIjrGif8oSygco?si=03f64ab820cc4e4f"><img src = "https://i.scdn.co/image/ab67616d00001e02c5ce7af35c36153b7e0a620c" alt='image_missing' width="300" height="300"></a>
<a href= "https://open.spotify.com/track/7FTf8uGI5O6hyu2WhIiUbV?si=ab5c7d1ed7804e72"><img src = "https://i.scdn.co/image/ab67616d00001e02b452406493a490a0369d4e05" alt='image_missing' width="300" height="300"></a>
<a href = "https://open.spotify.com/track/0YzFioWLGGYilHufj2JSw0?si=5ea1bc0b0aa34a37"><img src = "https://i.scdn.co/image/ab67616d00001e02eafcc7da794a5de0dc90d88c" alt='image_missing' width="300" height="300"></a>
<a href = "https://open.spotify.com/track/4QhMjrF69oIrscN7jc7vHm?si=7cf5fe66e171453a"><img src = "https://i.scdn.co/image/ab67616d00001e026ee4705dd8b0afdf7fcffd5b" alt='image_missing' width="300" height="300"></a>

## Centering Images

> ```html
> <div align="center"><img src = "https://link_to_image"></div>
> ```

<div align="center">
    <img src = "https://i.scdn.co/image/ab67616d00001e02c5ce7af35c36153b7e0a620c" alt='image_missing' width="300" height="300">
</div>

# Tables


> Think of the format as same as a pandas dataframe

> **Markdown**
> ```html
> |col 1|col 2|col3|              < first row denote column headers
> |-|--|------|                   < second row is just for delimiting headers from records(rows). Use '-' but notice how the number of '-' doesnt matter 
> |row1_1 |row1_2|---|            < first row of records, notice putting '---' gives you literal dash values now
> |N/A           |row2_2|row3_3|  < second row of records, notice how leading/trailing whitespace automatically controlled for
> ```


|col 1|col 2|col3|            
|-|--|-------|                 
|row1_1 |row1_2|---|
|N/A           |row2_2|row3_3| 

## Centering Table
> **Markdown**
> ```html
> <div align="center">
> 
> TABLE
> 
> </div>
> ```


<div align="center">

|col 1|col 2|col3|            
|-|--|-------|                 
|row1_1 |row1_2|---|
|N/A           |row2_2|row3_3|

</div>


# Emojis :joy: :heart:


## Find all the emojis [here](https://gist.github.com/rxaviers/7360908)

# Showable / Hidable Subsections


> Note that for header-like style, need to use the html `<h1>` `<h2>` styling instead of the `#`

<details>
<summary><h2>Subsection1</h2></summary>

Here is the content in subsection1

I can even include subsubsection

<details>
<summary><h3>SubSubSection1<h3></summary>

Here is the content in subsubsection1
</details>
</details>

<details>
<summary><h2>Subsection2</h2></summary>

Here is the content in subsection2

