# Style Guide <!-- omit in toc -->
#### [Lire le README](../../README.md) <!-- omit in toc -->
# Sommaire <!-- omit in toc -->
- [Naming system](#naming-system)
  - [Block](#block)
    - [1. Block (Composant global et indépendant)](#1-block-composant-global-et-indépendant)
      - [Examples](#examples)
  - [Element](#element)
  - [2. Element (Partie interne d’un Block)](#2-element-partie-interne-dun-block)
  - [Modifier](#modifier)
  - [3. Modifier (Variation ou État d’un Block/Element)](#3-modifier-variation-ou-état-dun-blockelement)
- [Architecture](#architecture)
  - [**Exemple**](#exemple)
- [Liste des classes préparé](#liste-des-classes-préparé)
  - [Elements](#elements)
    - [typography.css](#typographycss)
  - [Components](#components)
    - [btn.css](#btncss)
    - [input.css](#inputcss)
    - [card.css](#cardcss)
    - [navbar.css](#navbarcss)
  - [Utilities](#utilities)
    - [display.css](#displaycss)
  - [objects](#objects)
    - [grid.css](#gridcss)
- [Éléments du root](#éléments-du-root)



# Naming system
Nous utilisons la convention **[BEM](https://getbem.com/)** (Block, Element, Modifier) pour nommer les classes CSS.  

## Block
### 1. Block (Composant global et indépendant)  
Un **Block** représente un composant autonome.  

**Exemples de Blocks** :  
- `btn`  
- `card`  
- `nav`  
- `footer`  
- `header`  
#### Examples
```html
    <button class="btn">
        Ajouter
    </button>
```
## Element
## 2. Element (Partie interne d’un Block)
Un **Element** est une partie constitutive d’un Block.
Il se définit avec la syntaxe `block__element`.
**Exemples d'element** : 
- `btn__icon`
- `section__title`


```html
    <button class="btn">
        <i class="btn__icon">
            +
        </i>
        Ajouter
    </button>
```

## Modifier
## 3. Modifier (Variation ou État d’un Block/Element)
Un **Modifier** permet de représenter une variation ou un état particulier.
Il se définit avec la syntaxe `block--modifier`.
**Exemples de Modifier** : 
- `btn--primary` (style visuel différent)
- `btn--active` (état actif)
```html
    <button class="btn btn--primary">
        <i class="btn__icon">
            +
        </i>
        Ajouter
    </button>
```
<br />
<br />

# Architecture
Nous utilisons une architecture type **[ITCSS](https://www.freecodecamp.org/news/managing-large-s-css-projects-using-the-inverted-triangle-architecture-3c03e4b1e6df/)** (Inverted Triangle CSS)
## **Exemple**
```
/styles/
│
├── settings/ (variables, fonts, colors)/
│   ├── variables.css
│   └── themes.css
├── tools/ 
│   └── utilities.css
├── generic/ (reset, normalize)/
│   ├── reset.css
│   ├── elements/ (h1, p, a…)
│   ├── typography.css
│   └── link.css
├── objects/ (layout grid, containers)/
│   └── grid.css
├── components/ (btn, card, navbar…)/
│   ├── btn.css
│   ├── navbar.css
│   └── card.css
├── utilities/ (margin helpers, text-align…)/
│   └── display.css
└── pages/ (overrides spécifiques)/
    ├── homepage.css
    └── login.css
```


<br />
<br />

# Liste des classes préparé
## Elements
### typography.css
- `title`
- `subtitle`
- `surtitle`
- `text`

## Components
### btn.css
- `btn`
- `btn--pill`
- `btn--secondary`
### input.css
- `input`
### card.css
- `card`
### navbar.css
- `nav`


## Utilities
### display.css
- `d-flex`
- `flex-column`
- `flex-center`
- `text-center`
- `d-none`

## objects 
### grid.css
- `grid`
- `grid--2`
- `grid--3`


<br />
<br />

# Éléments du root

