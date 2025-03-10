# Themes

This repository is for the application themes and tools used across the [Hundred Rabbits](http://100r.co) [Ecosystem](https://github.com/hundredrabbits). 

<img src='https://raw.githubusercontent.com/hundredrabbits/Themes/master/PREVIEW.jpg' width='600'/>

## Setup

**Install Theme support** by adding [theme.js](https://github.com/hundredrabbits/Dotgrid/blob/master/desktop/sources/scripts/lib/theme.js) to your header. 

```
<script type="text/javascript" src="scripts/lib/theme.js"></script>
```

**Define Theme overrides** in a dedicated [theme.css](https://github.com/hundredrabbits/Dotgrid/blob/master/desktop/sources/links/theme.css) by adding this line to your header.

```
<link rel="stylesheet" type="text/css" href="links/theme.css"/>
```

**Initiate Theme support** by adding these lines somewhere in your project. The `Theme({background:#f00,..})` class takes a default theme as param, the `.install(element,callback)` method takes an element to append the `<style>` element to, and a param for a method called when the theme has been updated.

```
let theme = new Theme();
theme.install(document.body);
theme.start();
```

This will add an handler that will detect files dragged onto the project window, and append a `<style>` element to your document's body element with the theme overrides.

## Format Specs

The Theme format holds only 9 different colors.

- `background`, Application Background.
- `f_high`, Foreground, high-contrast.
- `f_med`, Foreground, medium-contrast.
- `f_low`, Foreground, low-contrast.
- `f_inv`, Foreground, inverted.
- `b_high`, Background, high-contrast.
- `b_med`, Background, medium-contrast.
- `b_low`, Background, low-contrast.
- `b_inv`, Background, inverted.

## The Theme Format

The Theme file format is a SVG file. The [theme.js](https://github.com/hundredrabbits/Dotgrid/blob/master/desktop/sources/scripts/lib/theme.js) loader will look for colors found in the element's `id` attributes. **Save the image on your computer and drag it** over the application window to install it.

### Example

![apollo](themes/apollo.svg)

### Content

```
<!-- Author: Unknown -->
<svg width="96px" height="64px" xmlns="http://www.w3.org/2000/svg" baseProfile="full" version="1.1">
  <rect width='96' height='64'  id='background' fill='#E0B1CB'></rect>
  <!-- Foreground -->
  <circle cx='24' cy='24' r='8' id='f_high' fill='#231942'></circle>
  <circle cx='40' cy='24' r='8' id='f_med' fill='#5E548E'></circle>
  <circle cx='56' cy='24' r='8' id='f_low' fill='#BE95C4'></circle>
  <circle cx='72' cy='24' r='8' id='f_inv' fill='#E0B1CB'></circle>
  <!-- Background -->
  <circle cx='24' cy='40' r='8' id='b_high' fill='#FFFFFF'></circle>
  <circle cx='40' cy='40' r='8' id='b_med' fill='#5E548E'></circle>
  <circle cx='56' cy='40' r='8' id='b_low' fill='#BE95C4'></circle>
  <circle cx='72' cy='40' r='8' id='b_inv' fill='#9F86C0'></circle>
</svg>
```

## Installation

Simply download these SVG files, and **drag and drop them onto the application window**, to install them.

### Dark

![apollo](themes/apollo.svg) ![orca](themes/orca.svg) ![battlestation](themes/battlestation.svg) ![soyuz](themes/soyuz.svg) ![lotus](themes/lotus.svg)

### Light

![coal](themes/coal.svg) ![marble](themes/marble.svg) ![snow](themes/snow.svg) ![swiss](themes/swiss.svg) ![tape](themes/tape.svg)

### Color

![mahou](themes/mahou.svg) ![pico8](themes/pico8.svg) ![frameio](themes/frameio.svg) ![berry](themes/berry.svg) ![commodore](themes/commodore.svg)

### Default

Included within `theme.js`.

![noir](themes/noir.svg) ![pale](themes/pale.svg)

## Supported Applications

- [Dotgrid](https://github.com/hundredrabbits/Dotgrid), vector tool.
- [Ronin](https://github.com/hundredrabbits/Ronin), pixel tool.
- [Orca](https://github.com/hundredrabbits/Orca), programing language.
- [Left](https://github.com/hundredrabbits/Left), writing tool.
- [Marabu](https://github.com/hundredrabbits/Marabu), music tool.
- [Donsol](https://github.com/hundredrabbits/Donsol), card game.
- [Paradise](https://github.com/hundredrabbits/Paradise), IF playground.
- [Pilot](https://github.com/hundredrabbits/Pilot), synthetiser.
- [Verreciel](https://github.com/hundredrabbits/Verreciel), space game.

This collection may also be used with:

- [Tape](https://aeriform.itch.io/tape) by Aeriform.
- [Memex](https://github.com/kormyen/memex) by Kormyen.
- [Autograph](https://github.com/jameschip/Autograph) by James Chip
- [Dot Matrix](https://github.com/lainsce/dot-matrix) by Lains

## Extras

You are welcome to submit your own themes to this collection!
