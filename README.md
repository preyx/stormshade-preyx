# PrEyX's ReShade Preset

Greetings from [twitch/xpreyx](https://www.twitch.tv/xpreyx)! This is my custom ReShade preset for Final Fantasy XIV

This is a preset meant for general gameplay, with optional DOF filters for screenshots.

I wanted a stream-friendly shader with improved contrast and color depth, but not too extreme in any direction as to render it un-watchable. It was originally developed for Stormshade 3 as a heavily modified Stormshade Vanilla preset, but I re-made it in Espresso Glow (GShade 2.x).

My PC setup is Intel i7-6700k, nVidia GTX1070. Game is set to 1080p, Borderless Windowed. This preset in its default state places a moderate load (~15%) on my GPU, but it is meant to keep me above 60fps everywhere except where there are super-high PC counts (Limsa Aetheryte Plaza, hunt trains, etc.).

**Notes:**
- Install [Espresso Glow v11](http://bit.ly/EspressoGlowV11) by [Espresso Lalafell](https://twitter.com/Espressolala). Install any available updates.
- Place "FF14-PrEyX.ini" in the "game\reshade-presets" folder.
- Activate the "FF14-PrEyX" preset and enjoy!
- I use the "High (Desktop)" FFXIV graphics preset with the following customizations:
  - Graphics Settings > General > Occlusion Culling > Off
  - Graphics Settings > General > Anti-aliasing > Off
    - Replace with forced FXAA in nVidia Drivers
  - Graphics Settings > General > Glare > Off
  - Graphics Settings > Shadow Quality > LOD > Off
  - Graphics Settings > Effects > Limb Darkening > Off
  - Graphics Settings > Effects > Radial Blur > Off

**When loading the preset for the first time, verify the order of filters are as follows:**
1. FFKeepUI
2. MXAOFFXIV
3. DepthHaze *(Off)**
4. ADOF *(Off)**
5. MotionBlur
6. FilmicSharpen
7. FilmicPass
8. Clarity
9. HDR *(Off)**
10. MultiLUT
11. Colorfulness
12. Lightroom *(Off)**
13. GaussianBlur
14. Curves
15. FFRestoreUI

\* *Off by default. More details below.*

**Too heavy for your system?** Disable MotionBlur for a slight performance boost and minimal visual sacrifice.

**Want more CONTRAST?** Enable HDR and Lightroom.

**Want more BLUR?** Enable DepthHaze and/or ADOF. I keybind ADOF for easy screenshotting effects.
