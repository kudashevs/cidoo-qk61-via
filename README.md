# CIDOO QK61 Layout

This repo contains my personal layout files for the CIDOO QK61 V2 keyboard and some useful links to get started.


## Before you start

Before using the layout files from this repo, make sure that your keyboard has the exact Vendor ID and Product ID. There
are different ways how you can do it. I would recommend using the Chrome browser because this is the easiest one.

Open Chrome browser, type `chrome://usb-internals` and open the "Devices" tab. There you will see a Vendor ID and Product ID.
These IDs are important to know because they are used in VIA definition files and [VIA uses them](https://caniusevia.com/docs/specification/)
to identify the keyboard when it is plugged in. If a definition file doesn't work, you can open it and check these IDs.

<img alt="Image" src="https://github.com/user-attachments/assets/f8d78b11-1f88-464f-9c5e-6d5c749cceb4" />

**Warning:** Make sure that the Vendor and Product IDs of your keyboard are identical to the presented ones.
