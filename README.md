# PrEyX's Stormshade Presets

Greetings from [twitch/xpreyx](https://www.twitch.tv/xpreyx)! This is my custom preset for the [Stormshade Reshade](http://stormshade.otakumouse.com/) plugin for Final Fantasy XIV

This is a preset meant for general gameplay, with an optional DOF filter for screenshots.

I wanted a stream-friendly shader with improved contrast and depth, but not too extreme in any direction as to render it un-watchable. It was originally developed for Stormshade 3 as a heavily modified Stormshade Vanilla preset, but I recently re-made it in Stormshade 4.

My PC setup is Intel i7-6700k, nVidia GTX1070. Game is set to 1080p, Borderless Windowed. This preset in its default state is GPU-intensive, but meant to stay above 60fps everywhere except where there are super-high PC counts (Limsa Aetheryte, hunt trains, etc.).

**Notes:**
- Install Stormshade using [Espresso Glow](http://bit.ly/EspressoGlowV9) by [Espresso Lalafell](https://twitter.com/Espressolala)
- Make sure the ini file is in the same directory as your ffxiv.exe
- I use the "High (Desktop)" graphics preset with the following customizations:
  - Graphics Settings > General > Occlusion Culling > Off
  - Graphics Settings > General > Anti-aliasing > Off
    - I use forced FXAA in nVidia Drivers
  - Graphics Settings > General > Glare > Off
  - Graphics Settings > Shadow Quality > LOD > Off
  - Graphics Settings > Effects > Limb Darkening > Off
  - Graphics Settings > Effects > Radial Blur > Off

**When loading the preset for the first time, verify the order of filters are as follows:**
1. FFXIV_UIDisplay_Top_Keep
2. FFXIV_MXAO
3. DepthHaze *(Off)**
4. ADOF *(Off)**
5. MotionBlur
6. FilmicSharpen
7. Tonemap
8. AmbientLight
9. Clarity
10. FFXIVMultiLUT
11. FilmicPass
12. HDR *(Off)**
13. LUT
14. Colorfulness
15. Lightroom *(Off)**
16. GaussianBlur
17. Curves
18. FFXIV_UIDisplay_Bottom_Restore

\* *Off by default. More details below.*

**Too heavy for your system?** Disable MotionBlur and AmbientLight for a performance improvement and minimal visual sacrifice.

**Want more CONTRAST?** Enable HDR and Lightroom.

**Want more BLUR?** Enable DepthHaze and/or ADOF. I keybind ADOF for easy screenshotting effects.
