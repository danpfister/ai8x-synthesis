# Keyword Spotting Demo

This Demo was modified for the course [227-0155-00L Machine Learning on Microcontrollers](https://www.vvz.ethz.ch/Vorlesungsverzeichnis/lerneinheit.view?lerneinheitId=172911&semkez=2023W&ansicht=LEHRVERANSTALTUNGEN&lang=en). The original README can be found in the file `Original_README.md`.

The model checkpoints and descriptions can be found in the [ai8x-training repository](https://github.com/danpfister/ai8x-training/tree/ml-on-mcu-project/project/kws_colours_final).

## Demo

The demo features a simple state machine using the keywords {`GO`, `STOP`, `RED`, `GREEN`, `BLUE`, `ON`, `OFF`}.

`GO` and `STOP` enable and disable the state machine, respectively. `RED`, `GREEN` and `BLUE` change which LED in the RGB LED D1 is currently selected. `ON` and `OFF` turns the selected LED on and off, respectively.

### Note

In `cnn.h` (which is generated automatically during synthesizing), the definitions `CNN_START`, `CNN_COMPLETE`, `SYS_START` and `SYS_COMPLETE` need to be commented out, as they interfere with the RGB LED usage.