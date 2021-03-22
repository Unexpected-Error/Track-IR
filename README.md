# Track-IR
DIY head tracking for flight and space sims

Contains files and images of my own track IR clip design as none of the current ones met my needs

Track IR is a method of tracking your head when playing space/plane/car sims to further immerse yourself by allowing you to look around virtually by moving your head.
It works by computing your location from 3 IR LEDs.

## Tools
* 3d printer
* solder

## Cost
* $13.22 + cost of PS3 eye

## BOM
* [electronics](https://www.mouser.com/ProjectManager/ProjectDetail.aspx?AccessID=ab94725237) - $4.68
* plastic - $1.44
* wire - 10¢
* [filter](https://www.peauproductions.com/products/infrared-light-high-pass-filter) - $2
* new lens (no longer sold, one without a IR cut filter will work) - $5
* PS3 eye (can get for cheap on ebay) [amazon](https://www.amazon.com/PlayStation-Eye-3/dp/B000VTQ3LU)

Rather than pay $170 (!) to have a few LEDs, plastic, and an IR camera shipped to my door, I started this project to see if I could accomplish it for cheaper. To do so you need a camera that can see IR, LEDs that emit IR (preferably in the spectrum your camera is most sensitive), software to compute your location based on the size and position of the 3 IR dots, and a plastic frame to hold the IR LEDs in place on you head.



## V1 - Proof of Concept
For the software, there is an open source project by the name of [open track](https://github.com/opentrack/opentrack)
For the camera, I took my webcam and taped on a visible light filter. Not having a proper filter, I used a floppy disk as it works well enough.
For the LEDs, I ordered them off of mouser (an online electronics retailer) [BOM](https://www.mouser.com/ProjectManager/ProjectDetail.aspx?AccessID=ab94725237)
For the plastic frame, I went with [this](https://www.thingiverse.com/thing:49142), a popular design for track IR, which I then 3d printed. 

### Circuit
<img src="/images/Circuit2.PNG" width="100"> <img src="/images/Circuit1.PNG" width="100">

### Camera
<img src="/images/Camera.jpeg" width="100">

### Demo + images
https://youtu.be/YlXVRmGuQ3A


<img src="/images/Mounted.jpeg" width="100"> <img src="/images/Working.jpeg" width="100">

### Results
The system did work, and so was a success, however:

The bottom two LEDs could not be seen by the camera when I tilted my head up

The floppy disk blocked out too much IR light, resulting in needing to replace batteries early, and having to turn the gain on the camera high enough that lots of noise was introduced

## V1.1 - Improvements
Sticking with the same software and camera, and with a new shipment of the LEDs, I replaced the plastic frame with another popular design. It mounts the LEDs to the side and away from my head ([thingverse](https://www.thingiverse.com/thing:2458689)) as to not be obstructed by my head. 

### Frame

<img src="/images/V1_1Frame1.jpeg" width="100"> <img src="/images/V1_1Frame2.jpeg" width="100">

### Results
This resulted in me being able to turn further before the camera lost line of sight to the LEDs, allowing me to turn down sensitivity for comfort

## V2 - Current 
I bought my own camera lense assembly and visible light filter ( [filter](https://www.peauproductions.com/products/infrared-light-high-pass-filter) ) and designed my own frame. I did this because V1.1 mounts on headphones, and I don't want to always have to wear headphones to play. This new version mounts on glasses, allowing me to use it more often. The new camera with a new lense assembly and light filter is to get a cleaner image of the LEDs for better tracking.

### Camera
<img src="/images/CameraUpdate1.jpeg" width="100"> <img src="/images/CameraUpdate2.jpeg" width="100">

### Frame

<img src="/images/V2Frame.jpeg" width="100">

### Demo
https://youtu.be/IIj-g7B0hHw 

### Results
While a lot of work went into the design, and it does work, the whole assembly is too heavy to be comfortable on glasses. Currently, I use V1.1's frame and LEDs, with V2's camera.




