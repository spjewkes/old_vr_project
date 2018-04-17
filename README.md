# Legacy DOS Virtual Reality Project

This is a very old copy of source code of a virtual reality project that I wrote way back in the 90s. It was written using a version of Borland Turbo C with it's BGI graphics drivers used for drawing the 3d scene.

*Please note this code has a number of issues.* It was written about 1 year after I started learning C. There are a number of things in here I'd certainly avoid doing these days. The reason I have uploaded this code is that I currently only have a hardcopy of this program. Therefore I decided to scan it in and at least have a softcopy for my own personal amusement.

I have no current intention of making this code compile. The only further changes I expect to make will be to fix futher problems with the scanning of the hardcopy.

## Technical details

A list of the technical details from what I can remember:

* This version used the TurboC BGI drivers. There was only a single buffer available for the 256 color mode that I used. I did modify this version later on to use a double-buffered ModeX version with my own graphics routines to remove the flicker. Sadly this version has been lost.

* There was no z-buffering at all. Each object was expected to have no concavities and so back-face culling using each surface normal should work. Objects were sorted very roughly based on a mid-point. It was not perfect by any means and was quite easy to get it to fail when a lot of objects were close together.

* The lighting was static. I believe it was lit just from above.

* The 256 color palette was cut into 16 color ranges. An object could be one of those 16 colors and then used the 16 shades available for that color.

* The collision detection was crude and used a sphere type collision detection from what I remember

