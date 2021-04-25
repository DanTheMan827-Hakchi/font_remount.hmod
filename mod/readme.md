# Font Remount

This module will search **/media/hakchi/fonts** and **/var/lib/hakchi/fonts** for font files with the following names

- title.fnt
- copyright.fnt
- debug.fnt
- small.fnt
- medium.fnt
- large.fnt

It comes with an extended title.fnt by default and will use that if no other is specified.

A description of the font files is as follows:

**title.fnt**  
This is the game title font

**copyright.fnt**  
This is used on the legal screen.

**small.fnt**  
This is used for the button legend and in tooltips.

**medium.fnt**  
This is used all over the UI.

**large.fnt**  
This is used for menu headings.


---
# Addionnal information to generate mini's compatible font .fnt file
**Use [BMFont](https://cdn.discordapp.com/attachments/381290855081967629/381291919797649408/bmfont64.exe) to generate the .fnt and .png files.**
1. **Options** > **Font settings**
    - Select a font, and set the _size_ to around 48 for a title font  
    - Turn on _font smoothing_ and super sampling to level 4  
    - Click "OK"  
    - Select the characters that you want to include on the right side of the window  

```
    Those sizes are only guidelines and some fonts may be smaller than others
           small.fnt - 24
          medium.fnt - 32
           title.fnt - 48
           large.fnt - 52
```

2. **Options** > **Export options**
    - Select 32-bit depth, and choose the _"Outlined text with alpha"_ preset
    - Choose _binary font descriptor_, and _png_ for texture format
    - Start with a texture width of 1024x512, click _"OK"_

3. **Options** > **Visualize**
    - If the title of the window indicates more than one sheet, close it and go back and increase the texture size a little bit until there's only one sheet
    - If there's only one and a lot of red at the bottom, you can decrease the size until it's gone.

4. **Options** > **Save bitmap font as...**

**Use [FntCombiner.exe](https://cdn.discordapp.com/attachments/381290855081967629/381291930081951744/FntCombiner.exe) to combine the two previous .fnt and .png files into a single .fnt that the classic can use.**


