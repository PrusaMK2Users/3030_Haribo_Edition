# Firmware

## Warning / Introduction

Depending on the y carriage you use (stock or aftermarket) your mileage might vary.  I will note where you need to make the necessary changes and how to determine the values, but be ready to shut down the machine if it looks like it's going to crash the head into the bed!

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

## Final step

Now compile and upload the firmware.. redo your xyz calibration as normal
