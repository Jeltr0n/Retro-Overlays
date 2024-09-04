# Jeltron's Retro Overlays
![ngpcsmall](https://github.com/Jeltr0n/Retro-Overlays/assets/70062490/a6099cd0-8d8b-46bb-b7ee-9abea6ce4279)


The goal with all of these overlays is to make the screen look as good as possible by blending how you remember it looking with what makes it look best.

## [640 x 480 Overlays for Retroarch](https://github.com/user-attachments/files/16769685/480p.overlay.set.zip)

353 devices, XX devices, ARC-D/S, 405m, 351v, RGB20s, RK2023, GKD Mini Plus

<details>
<summary>How to use</summary>

### Gameboy

- Video
  - Scaling
    - Integer= OFF
    - Aspect= Custom
      - X pos=80
      - Y pos=12
      - Width=480
      - Height=432
  - Bilinear filtering=off

- On-screen overlay
  - Preset: GB_DMG for greenscale, GB_Pocket for grayscale, GB_Bivert for Bivert simulation
  - Opacity=1.00

Palettes are applied based on the overlay
All will need:
- Core Options
  - GB colorization: Internal
	
GB_DMG
- Internal Palette: Pixelshift - Pack 1
- Pack 1 palette: Pixelshift 03 - BGB 0.3 Emulator

GB_Pocket
- Internal Palette: TWB Pack 2
- TWB Pack 2 Palette: 117 Silver Shiro

GB_Bivert
- Internal Palette: Pixelshift - Pack 1
- Pack 1 palette: Pixelshift 27- GBP Bivert

### Gameboy Advance

Video
- Scaling
  - Integer=OFF
  - Aspect=Custom
    - X pos=0
    - Y pos=0
    - Width=640
    - Height=427            
- Bilinear filtering=on

I suggest using this with a shader from the interpolation folder (choose what looks best to you)
If your device doesn't support shaders, try normal 2x video filter.

### NeoGeo

Video
- Scaling
  - Integer= OFF
  - Aspect= Custom
    - X pos=16
    - Y pos=08
    - Width=608
    - Height=448
- Bilinear filtering=optional

</details>


## [640 x 480 Overlays for Onion](https://github.com/user-attachments/files/16769499/480p.6-1-23.zip)
Miyoo Mini V1-3 & Plus

<details>
    <summary>How to use</summary>
    
How to use the Overlays with Onion
---
<details>
<summary>Game Boy</summary
                    
![prototype2](https://user-images.githubusercontent.com/70062490/231170138-b5b67517-9885-44d5-b51c-0b65d0dbb96d.png)

Please note that the 'GB-Pocket' gambatte palette requires Onion 4.2 beta 4 or later

This GP one is based on the work of @creamydips

**Quick Menu**
- Core Options
  - GB Colorization=  internal
  - Current category for palettes=  Essentials
  - Color Categories
    - Essentials=  (GB-DMG for the original green gameboy palette or GB-Pocket for the pocket grayscale palette)

**Settings**
- Video
  - Scaling
    - Integer Scale= ON
    - Keep Aspect Ratio= ON
  - Video Filter=  /GB-GBC/Filters for overlays/(DMG_GreenGrid for green color scheme, GBP_GrayGrid for gray pocket style)**
- On-Screen Display
  - On-Screen Overlay
    - Display overlay= ON
    - Overlay Preset=  /GB-GBC/GBOffset/**DMG_GBP (-Noise is an optional variant that replicates the reflective backing of the gb screen)**
    - Overlay Opacity=  1.00

I often put all of my GB and GBC roms in the same folder since they both use the gambatte core but you may want to separate them so that you can save different settings for them. Don't forget after you set your settings the way you want them to go to Overrides->Save Content Directory overrides or Retroarch will conveniently delete all of your settings. If you choose save core overrides it might save it for both GB and GBC which would not be ideal.
</details>

<details>
<summary>Game Boy Color</summary
                          
![prototype3](https://user-images.githubusercontent.com/70062490/231197229-5bcb7417-7ed5-4799-ae96-44bebcd2e927.png)

**Quick Menu**
- Core Options
  - Color Correction= GBC Only (set to OFF if you prefer ultra-saturated unrealistic colors)
  - Color Correction Mode= Accurate for very desaturated, Fast for mild desaturation 

**Settings**
- Video
  - Scaling
    - Integer Scale= ON
    - Keep Aspect Ratio= ON
  - Video Filter=  /GB-GBC/filters for overlays/**GBC_DarkGridReshade**
- On-Screen Display
  - On-Screen Overlay
    - Display overlay= ON
    - Overlay Preset=  /GB-GBC/GBOffset/**GBC**
    - Overlay Opacity=  1.00

</details>

<details>
<summary>Gameboy Advance</summary

![GBA_Example](https://user-images.githubusercontent.com/70062490/224847113-6c9af53f-40b8-494b-b2fc-ed412041305a.png)

**Quick Menu**
- Core Options
  - Color Correction= ON for realistic color, OFF for saturated color

**Settings**
- Video
  - Scaling
    - Integer Scale= OFF
    - Keep Aspect Ratio= ON
  - Video Filter=  /GBA/filters for overlays/**GBAOffset**
- On-Screen Display
  - On-Screen Overlay
    - Display overlay= ON
    - Overlay Preset=  GBA/GBAOffset/GBA_(Choose if you want grid or scanline)_(The number represents how opaque the effect will be)
    - Overlay Opacity=  1.00
   
</details>

<details>
<summary>Neo Geo Pocket</summary

![ms1st](https://user-images.githubusercontent.com/70062490/231246253-78d0598f-dde8-4fc2-bd5c-8bf45526b73f.png)

**Settings**
- Video
  - Scaling
    - Integer Scale= ON
    - Keep Aspect Ratio= ON
  - Video Filter=  GB-GBC\filters for overlays\GBC_DarkGridReshade (this is not a typo, same as GBC)
- On-Screen Display
  - On-Screen Overlay
    - Display overlay= ON
    - Overlay Preset= NGP/NGPOffset/NGP_Black
    - Overlay Opacity=  1.00
   
</details>

<details>
<summary>CRT</summary

![CRT_Example](https://user-images.githubusercontent.com/70062490/224847109-47166561-4230-4537-9790-9dbad8736952.png)

These are good for 4:3 systems scaled to full screen. 
Note: There was a bug in Onion's version of Retroarch that was fixed by @akouzoukos that made the overlays appear incorrectly. This bug is addressed in Onion 4.2 beta 4.

**Settings**
- Video
  - Scaling
    - Integer Scale= OFF
    - Keep Aspect Ratio= OFF
- On-Screen Display
  - On-Screen Overlay
    - Display overlay= ON
    - Overlay Preset= CRT/(Choose your favorite effect)
    - Overlay Opacity=  1.00

</details>

<details>
<summary>Scanlines & Grids</summary


Usually the 2px versions will be best for higher res systems.

**Settings**
- Video
  - Scaling
    - Integer Scale= (up to you)
    - Keep Aspect Ratio= (up to you)
- On-Screen Display
  - On-Screen Overlay
    - Display overlay= ON
    - Overlay Preset= Scanlines and Grids/(Choose your favorite effect)
    - Overlay Opacity=  1.00
</details>
  
</details>

## [750 x 560 Overlays](https://github.com/user-attachments/files/16822468/540p.zip)
Miyoo Mini V4 and up. 
Technically these are 752 x 560 because of how weird the screen is.
<details>
<summary>How to use</summary>

### Game Boy

For this one I have 3 options. DMG is a warts and all recreation of the original game boy's green screen, GBP is a nice grayscale one, and GB is greenscale but more readable than DMG

- Quick Menu
  - Core Options
    - GB Colorization: Internal
    - Current Color Category: Essentials for DMG/GBP, Extras for GB
    - Color Categories
      -Essentials: 'GB-DMG' for DMG overlay, 'GB-Pocket' for GBP overlay
      -Extras: 'BGB 0.3 Emulator' for 'GB' overlay
  - On-Screen Overlay
    - Overlay Preset: GB_540.cfg, DMG_540.cfg, or GBP_540.fcg depending on the palette you chose.
    - Overlay Opacity: You can change this to however intense you want the grid effect to be
- Settings
  - Video
    - Scaling
      - Integer Scale: OFF
      - Keep Aspect Ratio: ON
    - Video Filter: Normal/Normal 2x
   
### Game Boy Color

- Quick Menu
  - Core Options
    - Color Correction: GBC Only
    - Color correction mode: You can choose if you like fast or accurate more. Fast is more colorful. Accurate is more...accurate.
    - Dark Filter Level: 15% (This prevents pure white from looking way brighter than it is supposed to on original hardware)
  - On-Screen Overlay
    - Overlay Preset: GBC_540.cfg
    - Overlay Opacity: You can change this to however intense you want the grid effect to be
- Settings
  - Video
    - Scaling
      - Integer Scale: OFF
      - Keep Aspect Ratio: ON
    - Video Filter: Normal/Normal 2x
   
### Game Boy Advance

- Quick Menu
  - Core Options
    - Video
      - Color correction: Game Boy Advance
  - On-Screen Overlay
    - Overlay Preset: GBA_540.cfg
    - Overlay Opacity: You can change this to however intense you want the grid effect to be
- Settings
  - Video
    - Scaling
      - Integer Scale: OFF
    - Video Filter: GBA/Filter for Overlays/GBAOffset
    

<details>
    <summary>Miyoo Mini V4 overlay template</summary>
If you want to make your own overlay this could help you a bit. Please note: This is based on my screen but apparently some devices cut off the top row of pixels and others cut off the bottom row. It is probably safest to design your overlay to avoid both the top and bottom row. 
	
https://github.com/user-attachments/assets/86885277-e703-424a-8020-77f701c77d3d

</details>

</details>

## [720 x 720 Overlays](https://github.com/Jeltr0n/Retro-Overlays/files/13328709/720x720.Overlays.11-12-23.zip)
RGB30/20sx, RG Cube, Unicorn, Retropixel Pocket

<details>
    <summary>How to use</summary>

First set your aspect ratio to access manual control over the screen position:
- Settings->
    - Video->
        - Aspect Ratio->
            - Scaling->
                - Aspect Ratio->Custom

 <details>
    <summary>4:3</summary>
I have made some 600 x 800 and some 768 x 576 overlays for 4:3 systems. In my opinion it is better to have a screen crop than have a smaller picture on this screen. The 600 x 800 ones crop more of the screen so they are best to use in games with minimal UI or adjustable UI (a lot of arcade games for DC and PS1 have this in the options)

My favorite middle-ground is 768 x 576 which is 1.2x the size and only crops 24 pixels on either side. (because this screen is pretty high-res 24px is less than it sounds)
     
If an overlay says **576p** in the filename use these settings:
- X position: -24
- Y Position: 60
- Width: 768
- Height: 576

 If an overlay says **4:3 600x800** in the filename use these settings:
- X position: -40
- Y Position: 30
- Width: 800
- Height: 600

 If an is in the **480p** folder use these settings:
- X position: 40
- Y Position: 24
- Width: 640
- Height: 480

</details>

<details>
    <summary>Handhelds</summary>


<details>
    <summary>Gameboy</summary>
    
Scaling:
- X_Offset: 40
- Y_offset: 20
- Width: 640
- Height:576

</details>

<details>
    <summary>GBA</summary>
    
Scaling:
- X_Offset: 0
- Y_offset: 75
- Width: 720
- Height:480

</details>

<details>
    <summary>Neo Geo Pocket</summary>
    
Scaling:
- X_Offset: 40
- Y_offset: 30
- Width: 640
- Height:608

</details>

<details>
    <summary>Pokemini</summary>
    
Scaling:
- X_Offset: 0
- Y_offset: 102
- Width: 720
- Height:480
    
For this system it is not integer scaled so no overlay or video filter seems to add a nice pixel grid. 
The best method I have found to add a pixel grid is to go to Shaders->Handheld->Dot and set the following shader parameters:
- Gamma: 2.20
- Shine: 0.05
- Blend: 0.80

Don't forget to save your shader settings in the shader menu. For some reason they are not saved when you save overrides...

</details>

<details>
    <summary>Wonderswan</summary>
For wonderswan it is best to leave the aspect ratio set to 'core provided' and turn on integer scaling. This will allow you to press select to rotate the screen in games that require it. If you are wondering why the logos don't fill out more of the screen it is because the overlays are designed to avoid overlapping both the vertical and horizontal format. With this perfect 1:1 screen I wanted to make sure to retain that.
</details>

 
</details>

</details>

## [Game Boy Games](https://benjelter.itch.io)
If you are sick of playing the same old Gameboy games from 1993, I have made some new ones! :) 

Check them out on my itch page: https://benjelter.itch.io/
