# TP5000 MODULE HELPER

TP5000 module based on TP5000 2A 4.2V lithium/3.6V lithium iron battery charger, have built-in all external components needed for immediate use. Parameter setup is done using resistors, however, resistors silkscreen characters are unreadable and output pin labels are not exactly written as in the IC datasheet.

This document shows the equivalence between labels written in the module and in the IC [datasheet](assets/pdf/tp5000.pdf).

## The module in question

The only visible marking on the PCB is D14482, there are no references to the manufacturer. Silkscreens are unreadable.

![MODULE](/tp5000/assets/img/tp5000-module.jpg)

## Resistor map

The following image presents visually each resistor with both labels: IC manufacturer and module manufacturer.

![MODULE](/tp5000/assets/img/tp5000-resistors.svg)

## Pinout

The following image presents visually each header pin with a label exactly written as in the IC manufacturer datasheet.

![MODULE](/tp5000/assets/img/tp5000-pinout.svg)

## Module resistor values

The following tables show the values of the resistors that came soldered into the PCB. Those values are exactly the same found in the IC sample design pdf.

### VOLTAGE SELECTOR

| TP ID | PCB ID | MARK | VALUE |
|-------|--------|------|-------|
| CS    |  F     | NONE | OPEN  |

### CHARGE CURRENT

| TP ID | PCB ID | MARK | VALUE  |
|-------|--------|------|--------|
| RS a  |  SANYA | R100 | 0.1    |
| RS b  |  NONE  | NONE | OPEN   |

There are 2 pads in parallel for fine-tuning resistor value

### PRE-CHARGE CURRENT SETTING

| TP ID | PCB ID | MARK | VALUE |
|-------|--------|------|-------|
| Rtrick| NONE   | 0    | 0     |

Here are the configuration parameters obtained with the aforementioned resistor values:


| PARAMETER          | VALUE |
|--------------------|-------|
| VOLTAGE            | 3.6 V |
| CURRENT            | 1 A   |
| PRE-CHARGE CURRENT | 10%   |

