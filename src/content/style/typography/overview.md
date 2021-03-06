---
label: Style
title: Typography
tabs: ['Overview', 'Type Styles']
---

<page-intro>**Typography** is used to create clear hierarchies, useful organizations, and purposeful alignments that guide users through the product and experience. It is the core structure of any well designed interface.</page-intro>

## Typeface: IBM Plex

Carbon uses the new IBM open-sourced typeface, IBM Plex. It has been carefully designed to meet IBM's needs as a global technology company and reflect IBM's spirit, beliefs and design principles. IBM Plex can be accessed and downloaded from the <a href="https://github.com/ibm/type" target="blank">IBM GitHub repo</a>.

To use IBM Plex with Carbon components, simply toggle the scss variable `$css--plex` to true and components will automatically update.

```scss
$css--plex: true;
```

#### Sans-serif font stack

```scss
font-family: 'ibm-plex-sans', 'Helvetica Neue', Arial, sans-serif;
```

#### Monospaced font stack

```scss
font-family: 'ibm-plex-mono', 'Menlo', 'DejaVu Sans Mono', 'Bitstream Vera Sans Mono', Courier;
```

## Type scale

| rem       | px    | Actual size                  |
|-----------|-------|------------------------------|
| 0.75rem   | 12 px | Good design is good business |
| 0.875rem  | 14 px | Good design is good business |
| 1rem      | 16 px | Good design is good business |
| 1.125rem  | 18 px | Good design is good business |
| 1.25rem   | 20 px | Good design is good business |
| 1.5rem    | 24 px | Good design is good business |
| 1.75rem   | 28 px | Good design is good business |
| 2rem      | 32 px | Good design is good business |
| 2.25rem   | 36 px | Good design is good business |
| 2.625rem  | 42 px | Good design is good business |
| 3rem      | 48 px | Good design is good business |
| 3.375rem  | 54 px | Good design is good business |
| 3.75rem   | 60 px | Good design is good business |
| 4.25rem   | 68 px | Good design is good business |
| 4.75rem   | 76 px | Good design is good business |
| 5.25rem   | 84 px | Good design is good business |
| 5.75rem   | 92 px | Good design is good business |

### How it works

IBM designed a complementary type scale to use with IBM Plex. Each step on the scale is determined by the previous step on the scale. Mathematically it works out to the following:

```markup
X₂=X₁+{INT[(n-2)/4]+1}x2

X : step n type size     X₁ : step n-1 type size
```

The gap between two steps is always based on increments of two. It is a non-linear arithmetic progression, providing a smaller interval for smaller type and a larger interval for larger type, allowing for a wide range of scales. It provides sensible value and works well in a product environments.

## Typographic treatments

### Font weight

Font weight is an important typographic style that can add emphasis and is used to differentiate content hierarchy. Font weight and size pairings must be carefully balanced. A bold weight will always have more emphasis than a lighter weight font of the same size. However, a lighter weight font can rank hierarchically higher than a bold font if the lighter weight type size is significantly larger than the bold.

IBM Plex family provides a wide range of weights. However, only SemiBold, Regular, Light should be used for product design.

|  |  |
|--------------|------------|
| Font-weight: 300 / Light <br> _Should only be used at sizes greater than or equal to 18px / 1.125rem_  | Light 300  |
| Font-weight: 400 / Normal | Normal 400 |
| Font-weight: 600 / Semi-bold   | Semi-bold 600   |

### Body copy

We recommend using two sizes for body copy. The first is UI specific. To maximize screen real estate we chose a smaller 14px / 0.875rem body copy size for the standard UI console. However, for areas that have prolonged reading, like Documentation, we use a larger body copy size of 16px / 1rem to enhance readability.

|Body copy         | px   | rem     |
|------------------|-----|--------|
|Standard UI       |14px |0.875rem|
|Prolonged reading |16px |1rem    |

### Line-height

Line-height, traditionally known as leading, is one of several factors that directly contribute to readability and pacing of copy. Line-heights are based on the size of the font itself. Ideal line-heights for standard copy have a ratio of 1:1.5 (typesize : line-height). For example, a type at 16px/1rem would have a line-height of 1.5rem/24px (16 x 1.5). The exception to this rule are headings, which need less spacing and therefore have a line-height ratio of 1:1.25.

|Line-height       |Ratio  |
|------------------|-------|
|Standard UI       |1:1.5  |
|Headers           |1:1.25 |


### Line-length

Line-length, traditionally known as measure, is the number of characters in a single line. It also directly contributes to the readability and pacing of copy. Lines that are too long degrade eye tracking from line to line, making it difficult to gauge which line to read next. In contrast, lines that are too short make it difficult for a reader to maintain a steady reading rhythm. Short lines often create disproportionate ragged edges that negatively affect the design.

**Line-length: 52 - 78 characters**
