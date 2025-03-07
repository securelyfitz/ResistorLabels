# ResistorLabels

This script generates labels for resistor zip bags.

It is meant for AVERY 5260 or AVERY L7157 labels and 7x10cm (3"x4") zip bags.

The generated labels include:

-   Resistor value
-   4- and 5-band color codes
-   3- and 4-digit smd codes
-   EIA-96 smd code

<img src="Example.png">

# Usage

-   Install python3
-   Install the python3 library `reportlab`. This library is used to do the actual PDF generation.
-   Add your own required resistor values in `main()` of `LabelGenerator.py`.
-   If using Avery L7157, change the `layout` value in `main()` to `AVERY_L7157`.
-   Run the script `LabelGenerator.py`!

It will now generate a `ResistorLabels.pdf` that can be used to print onto AVERY 5260/L7157.

# More Details

This is forked from https://github.com/Finomnis/ResistorLabels

At first, I tried to make it a clean, PR'able option, but I got lazy halfway through.

I wanted just the color codes, big and bold, on both sides of the label. I used 4x4" 4 mil bags i had lying around, which fit nicely into a box I already had.

Labels are made to fold over the edge of the bag. They're repeated, not flipped, so the opening is always on the same side (left for me) and when you flip through the box, the labels always look right side up.

The original in turn is based on an idea from Zach Poff.

For more details on how to use these labels, visit his website:

https://www.zachpoff.com/resources/quick-easy-and-cheap-resistor-storage/
