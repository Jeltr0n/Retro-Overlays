# Jeltron's Retro Overlays
![prototype2](https://user-images.githubusercontent.com/70062490/231170138-b5b67517-9885-44d5-b51c-0b65d0dbb96d.png)

The goal with all of these overlays is to make the screen look as good as possible by blending how you remember it looking with what makes it look best.
## 640 x 480 Overlays
<details>
    <summary>Description</summary>

Systems: Miyoo Mini (Plus), 353v/vs, 353m, 35XX, ARC-D/S, 405m, 353ps, 351v, RGB20s, RK2023, GKD Mini Plus & many more

The instructions are for Onion but I will put general RetroArch Instructions as soon as I have time. It should be noted that only the Onion version of RA has the gambatte palettes that are ideal for the gameboy overlay. There is also a blending bug in RA that has been fixed in Onion's version of RA but might not be fixed in all versions of RA.

The GBP one is based on the work of @creamydips
</details>

### 2023-06-01 Update (https://github.com/OnionUI/Onion/files/11627966/6-1-23.update.zip)

<details>
    <summary>Changelog & Old Versions</summary>
Thanks to @duckyb

GB
- Fixed noise being present on the GBC overlay (that system did not have the same reflective backing as the DMG, so it didn't look authentic)
- Added Noise/No noise options for DMG

GBA
- fixed alignment issues w offset filter
- made scanlines and grid be better aligned with the frame. Note: It is impossible for the overlay to perfectly align with the pixel grid when it is not integer scaled. If this bothers you, I suggest a lower opacity or using integer scaling with the 2px scanlines overlay.
- made the rounded corners on overlay smoother so they look good on the Mini Plus
CRT
- removed some of the least useful filters (vertical checker, scanlines 2x)
- the vignette effect is now more subtle to avoid the screen getting too dark at the edges.
- the edges now have a smoother gradient
- the pixel patterns have been softened to not call too much attention to individual pixels on the larger screen of the miyoo mini plus
- a new overlay has been added for vertical arcade games. I don't know if it will fit everything correctly. Proportions were based on DoDonPachi
SFC
- a new overlay for Super Famicom by @duckyb
VIDEO FILTERS
-There is a very versatile new offset video filter by @eggs that allows you to offset the screen by X pixels by editing a simple text document. Could be useful for future overlays made by other people.

**4-4-2023 Update** [Jeltron Overlays- 480p.zip](https://github.com/OnionUI/Onion/files/11149108/Jeltron.Overlays-.480p.zip)
<details>
<summary>Changelog</summary>
- The GBA offset filter has been updated to align better with the overlays
- The GB logos have a slight blue added to give a stronger impression that they are white but in shadow rather than just dark gray
- The CRT filters have been completely redone. I didn't have enough time to make them good last time.
- A GBA grid filter has been added based on one that Miyoo included in their stock OS
</details>

Original set: [Onion Overlays.zip](https://github.com/OnionUI/Onion/files/10962300/Onion.Overlays.zip)
</details>
<details>
    <summary>How to use the Overlays with Onion</summary>
    
How to use the Overlays with Onion
---
<details>
<summary>Gameboy</summary
                    
![prototype2](https://user-images.githubusercontent.com/70062490/231170138-b5b67517-9885-44d5-b51c-0b65d0dbb96d.png)

Please note that the 'GB-Pocket' gambatte palette requires Onion 4.2 beta 4 or later

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
<summary>Gameboy Color</summary
                          
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

## Overlays for 720 x 720 screens
<details>
    <summary>Description</summary>
Systems: RGB30, Retropixel Pocket if you have one of the 5 that are out there
</details>



If you are sick of playing the same old Gameboy games from 1993, I have made some new ones! :) 
Check them out on my itch page: https://benjelter.itch.io/
