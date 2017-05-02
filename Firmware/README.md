# Firmware

## Introduction

The 3030 Haribo Edition frame has slightly more Z height than the stock Original Prusa i3 MK2. You will need to make some minor modifications to the firmware in order to accommodate for this.

## Warning

**Please Note:** Depending on the y carriage you use (stock or aftermarket), your mileage might vary.  Various y-carriages have different heights. I will note where you need to make the necessary changes and how to determine the values, but be ready to shut down the machine if it looks like it's going to crash the head into the bed!

## Configuration_prusa.h

Let's change the name of the printer:

```
// Printer name
#define CUSTOM_MENDEL_NAME "3030 Haribo Edition"
```

Let's set the correct Z_MAX_POS, the originial value is 210, and after a few test builds we determine 220 works

so let's set it to 220:

```
#define Z_MAX_POS 220
```
## Configuration.h

Since we are in here anyways, let's fix the encoder too:

```
#define ENCODER_PULSES_PER_STEP 2 // Increase if you have a high resolution encoder
#define ENCODER_STEPS_PER_MENU_ITEM 2 // Set according to ENCODER_PULSES_PER_STEP or your liking
```

to

```
#define ENCODER_PULSES_PER_STEP 4 // Increase if you have a high resolution encoder
#define ENCODER_STEPS_PER_MENU_ITEM 1 // Set according to ENCODER_PULSES_PER_STEP or your liking
```

## pins.h (optional)

Now depending which LCD board you have, you might find the rotary wheel direction is not intuitive (goes up when you expect down, down when up).  It's fairly easy to fix.  You need to invert 2 numbers in pins.h  

Find the first occurence of the following lines:
```
#define BTN_EN1 72
#define BTN_EN2 14
```

These are the atmega pin numbers assigned to the up and down motion of the menus.  To invert them, simply swap the numbers so the lines become:
```
#define BTN_EN1 14
#define BTN_EN2 72
```

## Final step

Now compile and upload the firmware.. redo your xyz calibration as normal
