# Universal Gas Flow Controller

**Universal Gas Flow Controller** is a desktop program for running gas experiments with mass flow controllers. It mixes hydrogen with nitrogen to the concentration you choose, runs timed exposure-and-purge sequences automatically, and shows live charts while recording all data for later analysis. Built-in safety checks stop the gas if anything goes wrong, and a simulator mode lets you practise without any hardware. It runs on Windows and macOS and was developed for a university project on optical hydrogen sensors.

## What it does

- **Set a hydrogen concentration** in ppm or %, and the program works out how much of each gas to send.
- **Run experiments automatically**: baseline, exposure and purge steps, repeated as many times as you like.
- **See what's happening**: live flows, concentration and timing at a glance, with clear warnings when a setting is outside what the equipment can do reliably.
- **Keep every measurement**: data is saved continuously, so nothing is lost if the computer stops.
- **Stay safe**: a big STOP ALL button, automatic stops when something goes wrong, and confirmations before risky actions.

## Getting started

**Windows (no installation):** extract `GasFlowController_1.0.0_Windows_offline.zip` to a short folder such as `C:\GasFlow`, then double-click `START_GAS_FLOW_CONTROLLER.bat`.

**Windows or macOS (with Python 3.10 or newer):** double-click `START_GAS_FLOW_CONTROLLER.bat` (Windows) or `START_GAS_FLOW_CONTROLLER.command` (macOS). The first start needs internet to install what the program needs; after that it works offline.

Then:
1. Open the gas cylinders first.
2. Connect each flow controller on the **Channels** tab (or choose **Simulator** to try it out).
3. Enter the gas in each cylinder, and start a mixture or a recipe.
4. Press **Start recording** on the **Data** tab before your experiment.

*Help → Quick guide and safety notes* inside the program explains the rest.

## Supported equipment

Xinnovis **MFC-E** and **S300 / S300D** mass flow controllers, connected over USB with the Xinnovis PSC converters. Tested on real hardware on 14 October 2026 (see [TEST_RESULTS_HARDWARE.md](TEST_RESULTS_HARDWARE.md)).

## Documentation

- [START_HERE.txt](START_HERE.txt): setting up on a new computer.
- [HANDOVER.md](HANDOVER.md): technical guide for developers.
- [TEST_RESULTS_HARDWARE.md](TEST_RESULTS_HARDWARE.md): test with the real equipment.

## Safety notice

This program controls flammable gas. It is a research tool, **not a certified safety system**. Always use stop valves, leak-checked tubing, ventilation and an independent hydrogen detector, and follow your laboratory's safety rules.

## Acknowledgements

The measurement approach follows H. M. Luong *et al.*, *Nature Communications* **12**, 2414 (2021). Device information comes from the manuals of Qingdao Xinnovis Microsystem Technology Co., Ltd.
