# [![UOFont](./img/UOFont.png)](https://jackkv.github.io/UOFont/)

I made a [demo](https://jackkv.github.io/UOFont/) that can also be used to share the font with others, just link them the website. `https://jackkv.github.io/UOFont/`

I created the font by tracing every pixel by hand in [Inkscape](https://gitlab.com/inkscape/inkscape), then i imported everything in [FontForge](https://github.com/fontforge/fontforge). It's a pixel-perfect replica.

I used a [WGL4 1.5](https://en.wikipedia.org/wiki/Windows_Glyph_List_4#Character_table) template, however, not every character was available in the game. It should still support most languages, as all the Latin, Greek, and Cyrillic characters are included.

 If you use this font in your project, please consider giving credit. Thanks.

## How to use

The font only works as intended when rendered at 20px, 15pt, or 1.25em.

If you don't care about keeping the classic outline, you can scale it by an integer to maintain the aspect ratio (20, 40, 60, etc.). Otherwise, you would first need to create the text as normal, apply the outline, then merge it into a layer and scale it as an image.

### In Photoshop

Be sure to disable text antialiasing then go into the text layer style and apply as shown.

![photoshop](./img/photoshop.png)

You need 7 strokes to have no transparent pixel, otherwise 3 are good enough.

### In Gimp

Disable text antialiasing and for the outline, i recommend using Filters > Light and Shadow > Drop Shadow as shown below.

![gimp](./img/gimp.png)

### In Web pages

I made a CSS outline, it only works if the font is set to 20px, 15pt, or 1.25em.

```css
    text-shadow: 
    0px -1px black, /* UP */
    0px 1px black, /* DOWN */
    -1px 0px black, /* LEFT */
    1px 0px black, /* RIGHT */
    -1px 1px black, /* UP LEFT */
    1px -1px black, /* UP RIGHT */
    -1px -1px black, /* DOWN LEFT */
    1px 1px black; /* DOWN RIGHT */
```

## Copyright

This is a fan project not affiliated with Electronic Arts or Broadsword.

Ultima Online™ is a trademark of Electronic Arts Inc.
