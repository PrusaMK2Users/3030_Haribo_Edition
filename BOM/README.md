# I. Intro
Below you will find the Bill of Materials for the 3030 Haribo Edition build. This list of materials is mostly complete, but it is still a work in progress. Please join our [Slack](http://codehemi.com) group and join the #haribo3030 channel if you have any questions at all.

# II. 3030 Frame Parts
Whether you are upgrading your existing Original Prusa i3 MK2 or building a 3030 Haribo Edition from scratch,
there are some aluminum extrusion parts that you will need. If you live in the United States, see our [CSV guide here](./MISUMI_CSV/README.md) to download a pre-made list of parts to upload and order straight from [Misumi US](https://us.misumi-ec.com/).

## Reference Parts List
If you would rather source the frame parts elsewhere, below is a list of all of the frame parts you will need and their part numbers from [Misumi US](https://us.misumi-ec.com/).

|Qty|Part #|Description|
|-----|-----|-----|
|3|HFSB6-3030-354-Z8-XA12-XB342|Black anodize 3030 Normal Rigidity Type extrusion 354mm 8mm counterbore hole @ 12mm and 342mm (x)|
|2|HFSB6-3030-320-TPW-Z8-XA100|Black anodize 3030 Normal Rigidity Type extrusion 320mm tap both ends 8mm counterbore hole @100mm (y)|
|2|HFSB6-3030-330-TPW|Black anodize 3030 Normal Rigidity Type 330mm tap both ends (z)|
|1|HFSB6-3030-200-Z8-XA15|Black anodize 3030 High Rigidity Type extrusion 200mm 8mm counterbore hole @ 15mm (spool holder vertical)|
|1|HFSB6-3030-147-LTP|Black anodize 3030 High Rigidity Type extrusion 147mm tap left end (spool holder horizontal)|
|2|PSFG8-370|Hard Chrome Precision Linear Shaft - Straight 370mm (x)|
|2|PSFG8-360|Hard Chrome Precision Linear Shaft - Straight 360mm (y)|
|2|PSFG8-320|Hard Chrome Precision Linear Shaft - Straight 320mm (z)|

# III. Other Hardware
TODO fill this out

# IV. Bushings (OPTIONAL)
If you are upgrading from an Original Prusa i3 MK2, you may re-use the LM8UU bushings for X, Y and Z axes. However, you may consider swapping the X and Y axes with IGUS Drylin bushings. You can find the quantity and description below.

## Igus bushings
|Qty|Part #|Description|
|-----|-----|-----|
|6|RJ4JP-01-08|IGUS DRYLIN® Bushing|


# IV. Scratch Build
The remainder of this document is geared towards individuals who would like to build an entire 3030 Haribo Edition from scratch

## Prusa Research

|Qty|Part #|Description|
|-----|-----|-----|
|1|PRI-UPG-MK2-ORG|Original Prusa i3 Plus to MK2 upgrade kit|

## Electronics

|Qty|Source|Description|
|-----|-----|-----|
|1|ultimachine|Rambo Mini v1.3
|1|eBay / aliexpress|AC 110V-220V TO DC 12V Switch Power Supply 20A or 30A|
|1|eBay / aliexpress|IEC power socket|
|1|eBay / aliexpress|Power switch|
|1|e3d|50x50x15mm 12v DC Side Blow Fan|
|1|eBay / aliexpress|Smart controller Reprap 2004 LCD|
|2|eBay / aliexpress|2x5 ribbon cable (>40cm)|
|-|Electronics store|14awg power wire (black/red)|
|-|Electronics store|14awg ferrules|

- if you use the mk1-> mk2 upgrade kit you will need to get the above, otherwise you can reuse from the mk2 kit
- I would consider ferrules __essential__ to ensure the wires are properly terminated for the power blocks

## Misc hardware

```
================================================================================
= Some of the hardware listed below you can reuse if you have the full mk2 kit =
= Some fo the hadrware listed is *partially* in the mk1->mk2 kit               =
=                                                                              =
= I listed *all* the hardware used, it's up to you to take stock what you need =
================================================================================
```

|Qty|Source|Description|
|-----|-----|-----|
|-|Electronic store|Short zip ties (just get a bag full)|
|8|McMaster / Fastenal|M3 fender washer|
|2|McMaster / Fastenal|M5 fender washer|
|4|McMaster / Fastenal|M2 washer|
|14|McMaster / Fastenal|M3 washer|
|36|McMaster / Fastenal|M6 washer|
|6|McMaster / Fastenal|M3 square nut|
|2|McMaster / Fastenal|M3 lock nut|
|9|McMaster / Fastenal|M3 hex nut|
|4|McMaster / Fastenal|Socket Head Cap Screw M2 x 12mm|
|15|McMaster / Fastenal|Socket Head Cap Screw M3 x 10mm|
|6|McMaster / Fastenal|Socket Head Cap Screw M3 x 12mm|
|10|McMaster / Fastenal|Socket Head Cap Screw M3 x 18mm|
|3|McMaster / Fastenal|Socket Head Cap Screw M3 x 20mm|
|2|McMaster / Fastenal|Socket Head Cap Screw M3 x 25mm|
|3|McMaster / Fastenal|Socket Head Cap Screw M3 x 30mm|
|3|McMaster / Fastenal|Socket Head Cap Screw M3 x 40mm|
|5|McMaster / Fastenal|Button Head Cap Screw M3 x 8mm|
|4|McMaster / Fastenal|Button Head Cap Screw M3 x 10mm|
|2|McMaster / Fastenal|Button Head Cap Screw M3 x 12mm|
|4|McMaster / Fastenal|Button Head Cap Screw M4 x 6mm|
|9|McMaster / Fastenal|Socket Head Cap Screw M8 x 40mm|
|12|McMaster / Fastenal|Socket Head Cap Screw M6 x 12mm|
|54|McMaster / Fastenal|Socket Head Cap Screw M6 x 14mm|
|4|McMaster / Fastenal|Socket Head Cap Screw M6 x 20mm|

- M6x12mm screws should be used for the parts that have recessed holes.  Namely: Y idler and motor holder, the Rambo mount holder and the Z Rod Holders
- most places sell hardware in packs of 50 or 100.. for most of these you might as well get them in bulk
- the y carriage is any standard square type that you can get for a generic prusa i3
- the 5x16 shaft can be found in lots of RC off road buggies

## "Missing bits"

- if you used the mk1->mk2 upgrade kit, you will find that you are missing a whole bunch of stuff Prusa assume you will reuse from your non-existant mk1
- this is where I will be documenting the missing bits *I* used .. you can always substitute your own ideas

|Qty|Source|Description|Why?|
|-----|-----|-----|-----|
|-|Electronic store|Wire loom (3/8" or 10mm)|wire management|
|1|eBay / aliexpress|Prusa i3 Universal Y Carriage Plate|mounting the heatbed|
|2|eBay / aliexpress|GT2 16T pulley||
|4|eBay / aliexpress|F623ZZ 3x10x4mm flanged bearing|put two of them together so the flange size faces out as belt idler|
|1|eBay / Hobby Store|HPI Blitz / Firestorm Titanium Idler Gear Shaft 5x16m #104138|extruder idler bearing rod|
|1|eBay / aliexpress|625 5x16x5mm bearing|bearing in the extruder idler|
|2|eBay / aliexpress|Extruder spring ID 3.5mm OD 5mm Height 21.5mm|springs for the extruder idler|
|4|eBay / aliexpress|LM8UU linear bearing|bearing for the x ends|
