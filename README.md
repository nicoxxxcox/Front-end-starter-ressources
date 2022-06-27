<p align="center">A curated list of needed tools when start a Front-end project</p>

# Fonts
* [Transfonter](https://transfonter.org/) - _@fontface generator_
* [Googlefonts](https://fonts.google.com/) - _CDN for fonts_
* [System font stack](https://systemfontstack.com) - _Basic system font stacks_

# Buttons
* [Building a button component](https://web.dev/building-a-button-component/) - _A foundational overview of how to build color-adaptive, responsive, and accessible <button>button</button> components._

# Sizes scaling
* [Min-Max-Value Interpolation calculator](https://min-max-calculator.9elements.com/) - _Create fluid scales for type and spacing_
* Container with min() function : `width: min(100% - 2rem, 1200px);`


# Reset/Normalize
* [Normalize by @necola](https://github.com/necolas/normalize.css) - _A modern alternative to CSS resets_
* [Mini-reset by @jgthms](https://github.com/jgthms/minireset.css) - _A tiny modern CSS reset_

# Methodology
* [BEM](https://9elements.com/bem-cheat-sheet/) - _Even the most experienced CSS developers don't always find the right class name_
* [Guide de code (par @mdo)](https://pixelastic.github.io/code-guide/) - _An HTML and CSS standard_

# Grid
| Size | Min    | Max    | Cols | Margin  | Gutter |
|------|--------|--------|------|---------|--------|
| xs   | 320px  | 639px  | 4    | 16px    | 16px   |
| sm   | 640px  | 899px  | 8    | 30px    | 16px   |
| md   | 900px  | 1199px | 12   | 50px    | 16px   |
| lg   | 1200px | 1599px | 12   | 90px    | 24px   |
| xl   | 1600px | \-     | 12   | \>180px | 24px   |

# Layouts
* [Css layouts](https://csslayout.io/) - _Popular layouts and patterns made with CSS_
* [Clever Grid system with grid](https://medium.com/@aparnamovva/12-modern-css-techniques-for-older-css-problems-df4d6d543fea#69cc) - _Replacing The Older Grid System_  ⬇️ :
```css
--minColumnWidth: 22.5rem; /* 360px/16px */
--grid-gap: 1rem;
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(min(var(--minColWidth), 100%), 1fr));
  grid-gap: var(--grid-gap) ;
}
```
It give : 

![Alt text](https://miro.medium.com/max/700/1*Td7psaqT8PHzKeHo806XnQ.png "grid result")

* Auto-grid all childs ⬇️ :
```css
--minColumnWidth: 22.5rem; /* 360px/16px */
--grid-gap: 1rem;
@media (min-width: var(minColumnWidth)){
  .auto-grid {
    display: grid;
    grid-gap: var(--grid-gap) ;
    grid--auto-flow: column;
    grid-auto-columns: 1fr;
  }
}
```



# Mobile
* [Dealing with hover on mobile (video)](https://www.youtube.com/watch?v=uuluAyw9AI0) - _We can't hover on mobile devices, so what can we do about hover animations and other things that we might need to have on laptops and desktops?_