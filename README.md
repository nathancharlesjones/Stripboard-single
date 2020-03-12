# Stripboard prototpying PCB
![](https://github.com/nathancharlesjones/Stripboard-single/blob/master/Stripboard-Single_PCB.png)

# How to order
1. Download or clone this repository.
2. Follow [these instructions for ordering an assembled PCB from JLCPCB or MakerFabs](https://github.com/nathancharlesjones/Embedded-for-Everyone/wiki/3.-Building-a-circuit-on-a-PCB-and-connecting-it-to-the-rest-of-the-embedded-device#ordering-an-assembled-pcb).

This board was also designed with large-enough dimensions to be manufactured by hand using a PCB mill or other manual technique.

The cost is approximately $0.50 per board on JLCPCB (in quantities of 10).

# PCB Silkscreen Text
> - Max current: 3.5A (temp rise: 35 deg C)
> - Max voltage: 100V (70 V_AC RMS)
> - For more information: github.com/nathancharlesjones/Embedded-for-Everyone/wiki

## Notes about the silkscreen text
- Current
   - Max current was calculated using the [4PCB Trace Width Calculator](https://www.4pcb.com/trace-width-calculator.html) with the following parameters:
     - Trace width: 32 mils (given)
     - Thickness: 1 oz/ft^2 (assumed)
     - Temperature rise: 35 deg C (assumed)
     - Ambient temperature and trace length have no affect on the result.
   - You can increase the copper thickness to 2 oz/ft^2 to roughly double the current carrying capacity of the PCB traces (may incur additional cost from your PCB manufacturer).
- Voltage
   - Max voltage was calculated using the [SMPS voltage clearance calculator](https://www.smps.us/pcbtracespacing.html) with the following parameter:
     - Spacing, external layer: 24 mils (given)
   - This was measured using Eagle at the nearest points between two adjacent pads (which was determined by me to be the smallest clearance) and also confirmed by inspecting the pad diameter for the part in question (74 mils).
