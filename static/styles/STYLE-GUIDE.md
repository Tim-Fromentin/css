# Style Guide
#### [Lire le README](../../README.md)
# Sommaire

- [Naming system](#naming-system)
  - [Block](#block)
  - [Element](#element)
  - [Modifier](#modifier)
- [Architecture](#architecture)
- [Liste des classes préparé](#liste-des-classes-préparé)
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
- `btn--primary`
- `btn--secondary`
### card.css
- `card`
### navbar.css
- `nav`


## Utilities
### display.css
- `d-flex`
- `d-grid`


<br />
<br />

# Éléments du root

