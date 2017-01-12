# Firmware

## Warning / Introduction

Depending on the y carriage you use (stock or aftermarket) your mileage might vary.  I will note where you need to make the necessary changes and how to determine the values, but be ready to shut down the machine if it looks like it's going to crash the head into the bed!

## Determine max z height

The default max z height is 210mm.  The 3030 Haribo Edition configuration allows a higher z height (up to 226mm on my reference build).

You can determine your max during xyz calibration.  When it ask you to raise the z carriage all the way up to top, raise it up to 210mm as you measure from the tip of the hotend to the heatbed. then go up one or two more times.  This should put you in a safe spot.

Continue the calibration as normal. When it starts to lower the z carriage, get ready to turn off the machine in case it starts to touch the heatbed.

After it finish the calibration, use "move axis" to move the z all the way up to the top.

Measure from the top of the x end to the bottom of the z rod mount (on mine i measured 16mm)

this is your extra z height

## Configuration_prusa.h

Let's change the name of the printer:

```
// Printer name
#define CUSTOM_MENDEL_NAME "3030 Haribo Edition"
```

Let's set the correct Z_MAX_POS, the originial value is 210 and our extra z height is 15, so let's set it to 226:

```
#define Z_MAX_POS 226
```

then just compile and upload the firmware.. redo your xyz calibration as normal
