# CIDOO QK61 Layout

This repo contains my personal layout files for the CIDOO QK61 V2 keyboard and some useful links to get started.


## Before you start

Before using the layout files from this repo, make sure that your keyboard has the exact Vendor ID and Product ID. There
are different ways how you can do it. I would recommend using the Chrome browser because this is the easiest one.

Open Chrome browser, type `chrome://usb-internals` and open the "Devices" tab. There you will see a Vendor ID (VID) and
Product ID (PID). These IDs are important because they are used in VIA definition files and [VIA uses them](https://caniusevia.com/docs/specification/)
to identify the keyboard when it is plugged in. If a definition file doesn't work, you can open it and check these IDs.

<img alt="USB internals" src="https://github.com/user-attachments/assets/f8d78b11-1f88-464f-9c5e-6d5c749cceb4" />

**Warning:** Make sure that the Vendor and Product IDs of your keyboard are identical to the presented ones.


## Using VIA 

The **first step** is to open the VIA software and connect the keyboard using an appropriate definition file. In my case,
the definition file from EPOMAKER site didn't work (it is for devices with "0x28e9" VID and "0x3008" PID which seems to
be the first version of the keyboard). So, I found the appropriate CIDOO QK61 V2 JSON file on the [CIDOO site](https://cidootech.com/pages/downloads).

<img width="80%" alt="VIA Settings" src="https://github.com/user-attachments/assets/66460e99-3912-497b-9562-2bcec6165bad" />

The **second step** is to use the VIA software to update the keyboard's layout. I would recommend using the Chrome browser again.
Open the [VIA site](https://caniusevia.com/) and click on the "Try Now!" link. When the page is loaded, go to the "Settings"
section and click on "Show Design tab" (we are going to use it for the definition file) and pick "3D" in the Render Mode
(there is a bug with the 2D mode, so the VIA might work or might not).

<img width="80%" alt="VIA Design" src="https://github.com/user-attachments/assets/5fa52b94-ef8a-45f4-bca7-4d6314210427" />

Then, open the "Design" and load the appropriate definition file that we downloaded before. If everything worked as intended,
you will see CIDOO QK61 in the "Shown Keyboard Definition". Now, you can authorize your device and get ready to remap it.

<img width="80%" alt="VIA Authorize device" src="https://github.com/user-attachments/assets/5f13f7c9-187d-42cc-9390-0550b18dadc5" />

<img width="80%" alt="VIA Configure" src="https://github.com/user-attachments/assets/348068f9-39f5-47c8-9c1a-36476de36eb4" />
