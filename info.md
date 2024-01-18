# Grahpics Information File

It is important to note that this graphic standard is indeed very new and embryonic. Information is few but well studied.

## What does the archive contain
It contains backgrounds and logos that can be used in traditional 2d reaster software, which is the supposed workflow to match with (I.E. PhotoShop, Gimp, Paint3D). 

The folder is simple but practical (hopefully).

## Color Scheme
The color theme may be rapresented as a linear gradient between colour like:
    magenta - cyan
    deep violet - deep blue

### in RGB SETTING, for the gradient to be valid:
- Blue must be locked to a number N (0 - 255 / 0.0 - 1.0)
- Red + Green must be equal to N
    
> NOTE: avoid pastel colours, it is meant to give a neon vibe: synthwave colour palette without the 80s grahpics

## Model and Geometry
We **exploit** low poly 3D modelling and metal/glass refractions, it has become integral part of the branding.
Indeed, none of the provided assets were made with 2D raster tools.

By "low poly" it is meant flat shaded regular models that celebrate the computed perfection of reflections, by applying metallic or glasslike (Beckmann or Multiscatter GGX) raytraced shaders, creating a crystaline structure.

Lightning is standard only for a sky model, which is described in the example workflow.

## Example workflow
- Raytraced Atmospheric simulation (Nishita Sky) resembling space:
    - Ozone at maximum
    - Either Dust at 0.01 or Air at 0.01

- Backgrounds Elements:
    - Here lays programming freedom, procedural generation, physics simulations or advanced shaders
    - Usually a procedurally generated object may be layered (not composited) on a background image

- PostProcessing:
    - HeavenParty may not oversaturate or make heavy usage of raster effects, procedural meshes are the strengths of it really
    - But it may gloom

- Composition:
    - Logo may be applied on it AFTER or DURING rendering (as an in-scene object or layered image)

> Obviously, render Engine may be set to CYCLES

> Only variations of the backgrounds were provided for the sake of simplicity, tho feel free to ask for any other more specific assets given the context.

> Later on in this folder there will be also provided .blend files containing example data of the branding, as well as the file readers for eventual prioritary software developed by HeavenParty's internal staff.


Thank you very much for your cooperation.
Sylvio@HeavenParty