# CIDOO QK61 Layout

This repo contains my personal layout files for the CIDOO QK61 V2 keyboard and some useful links to get started.


## Before you start

Before using the layout files from this repo, make sure that your keyboard has the exact Vendor ID and Product ID. There
are different ways how you can do it. I would recommend using the Chrome browser because this is the easiest one.

Open Chrome browser, type `chrome://usb-internals` and open the "Devices" tab. There you will see a Vendor ID (VID) and
Product ID (PID). These IDs are important because they are used in VIA definition files and [VIA uses them](https://caniusevia.com/docs/specification/#vendor--product-id)
to identify the keyboard when it is plugged in. If a definition file doesn't work, you can open it and check these IDs.

<img alt="USB internals" src="https://github.com/user-attachments/assets/f8d78b11-1f88-464f-9c5e-6d5c749cceb4" />

**Warning:** Make sure that the Vendor and Product IDs of your keyboard are identical to the presented ones.


## Using VIA 

The **first step** is to open the VIA software and connect the keyboard using an appropriate definition file. In my case,
the definition file from EPOMAKER site didn't work (it is for devices with "0x28e9" VID and "0x3008" PID which seems to
be the first version of the keyboard). So, I found the appropriate CIDOO QK61 V2 JSON file on the [CIDOO site](https://cidootech.com/pages/downloads).

<p align="center">
<img width="80%" alt="VIA Settings" src="https://github.com/user-attachments/assets/66460e99-3912-497b-9562-2bcec6165bad" />
</p>

The **second step** is to use the VIA software to update the keyboard's layout. I would recommend using the Chrome browser again.
Open the [VIA site](https://caniusevia.com/) and click on the "Try Now!" link. When the page is loaded, go to the "Settings"
section and click on "Show Design tab" (we are going to use it for the definition file) and pick "3D" in the Render Mode
(there is a bug with the 2D mode, so the VIA might work or might not).

<p align="center">
<img width="80%" alt="VIA Design" src="https://github.com/user-attachments/assets/5fa52b94-ef8a-45f4-bca7-4d6314210427" />
</p>

Then, open the "Design" and load the appropriate definition file that we downloaded before. If everything worked as intended,
you will see CIDOO QK61 in the "Shown Keyboard Definition". Now, you can authorize your device and get ready to remap it.

<p align="center">
<img width="80%" alt="VIA Authorize device" src="https://github.com/user-attachments/assets/5f13f7c9-187d-42cc-9390-0550b18dadc5" />
</p>
<p align="center">
<img width="80%" alt="VIA Configure" src="https://github.com/user-attachments/assets/348068f9-39f5-47c8-9c1a-36476de36eb4" />
</p>


## Layouts

As you might know, I am a big fan of Vim. So, my personal layout is influenced by it. However, not all the mappings are Vim
related and come from different sources. In this repository you will find the following layout files:
- [default layout](#default) - the default keyboard layout (in case something goes bad)
- [Vim-like layout](#vim-like) - this is my layout which is heavily influenced by Vim
- [extended layout](#extended) - this is an extended layout for those who miss the arrow keys


**Warning:** I don't really care about RBGs, lighting and other light-related stuff. Some light-related keys might be
overwritten because I didn't pay much attention to those keys while I thought about remapping. 

### <a id="default">Default layout

You can find information about the default layout in [the manual](https://epomaker.com/blogs/manuals/cidoo-qk61-manual). In my case,
the layout was a little different from what is in the manual. In addition, it was a bit surprising for me because I expected
the FN key to be in a different position. As you can see in the first picture, the FN key is on the very bottom right.

<p align="center">
<img alt="Layer 0" src="https://github.com/user-attachments/assets/c0fc3218-a72a-49c1-93d4-36235e8394be" />
<img alt="Layer 2" src="https://github.com/user-attachments/assets/0ca1d060-5079-4349-8c80-9cbbceb96716" />
</p>

| Key/Key combination | Key    | Description                                                           |
|---------------------|--------|-----------------------------------------------------------------------|
| FN+Z                |        | Toggle LOGO LED light mode                                            |
| FN+X                |        | Toggle LOGO LED light color                                           |
| FN+Space            |        | Toggle ON/OFF Backlight (different from the manual)                   |
| FN+Backspace        |        | Reset the keyboard to the factory setting (different from the manual) |
| &nbsp;              |        |                                                                       |
| FN+A                |        | Windows System                                                        |
| FN+S                |        | Mac System                                                            |
| &nbsp;              |        |                                                                       |
| Esc                 | Esc    | Esc                                                                   |
| FN+Esc              | `      | Backtick                                                              |
| FN+1                | F1     | F1                                                                    |
| FN+2                | F2     | F2                                                                    |
| FN+3                | F3     | F3                                                                    |
| FN+4                | F4     | F4                                                                    |
| FN+5                | F5     | F5                                                                    |
| FN+6                | F6     | F6                                                                    |
| FN+7                | F7     | F7                                                                    |
| FN+8                | F8     | F8                                                                    |
| FN+9                | F9     | F9                                                                    |
| FN+0                | F10    | F10                                                                   |
| FN+-_               | F11    | F11                                                                   |
| FN+=+               | F12    | F12                                                                   |
| FN+T                | PrtSc  | Print Screen                                                          |
| FN+Y                | Scroll | Scroll                                                                |                
| FN+U                | Pause  | Pause                                                                 |
| &nbsp;              |        |                                                                       | 
| FN+G                | Ins    | Insert                                                                |
| FN+B                | Del    | Delete                                                                |
| FN+H                | Home   | Home                                                                  |
| FN+N                | End    | End                                                                   |
| FN+J                | PgUp   | Page Up                                                               |
| FN+M                | PgDn   | Page Down                                                             |
| &nbsp;              |        |                                                                       |
| FN+/?               | Up     | Up                                                                    |
| FN+App              | Down   | Down                                                                  |
| FN+RAlt             | Left   | Left                                                                  |
| FN+RCtrl            | Right  | Right                                                                 |

Download the [default layout](layouts/default-cidoo_qk61.layout.json) - use "Download as raw file".

### <a id="vim-like">Vim-like layout

This is my personal layout which I use on an everyday basis. Pay attention that I remapped CapsLock to Esc. In addition,
this layout does not have the possibility to use the 3rd layer.

<p align="center">
<img alt="Layer 0" src="https://github.com/user-attachments/assets/2fc8ac6d-b188-4eb8-b35a-b9f805448694" />
<img alt="Layer 2" src="https://github.com/user-attachments/assets/13d8b6c7-d59f-4f2f-81a4-0893284f770a" />
</p>

| Key/Key combination | Key    | Description                                                           |
|---------------------|--------|-----------------------------------------------------------------------|
| FN+[                |        | Toggle LOGO LED light mode                                            |
| FN+]                |        | Toggle LOGO LED light color                                           |
| FN+Space            |        | Toggle ON/OFF Backlight                                               |
| FN+Backspace        |        | Reset the keyboard to the factory setting                             |
| &nbsp;              |        |                                                                       |
| -                   |        | Windows System (I don't need it)                                      |
| -                   |        | Mac System (I don't need it)                                          |
| &nbsp;              |        |                                                                       |
| CapsLock            | Esc    | Esc                                                                   |
| FN+Esc              | Esc    | Esc                                                                   |
| Esc                 | `      | Backtick                                                              |
| FN+1                | F1     | F1                                                                    |
| FN+2                | F2     | F2                                                                    |
| FN+3                | F3     | F3                                                                    |
| FN+4                | F4     | F4                                                                    |
| FN+5                | F5     | F5                                                                    |
| FN+6                | F6     | F6                                                                    |
| FN+7                | F7     | F7                                                                    |
| FN+8                | F8     | F8                                                                    |
| FN+9                | F9     | F9                                                                    |
| FN+0                | F10    | F10                                                                   |
| FN+-_               | F11    | F11                                                                   |
| FN+=+               | F12    | F12                                                                   |
| FN+T                | PrtSc  | Print Screen                                                          |
| FN+Y                | Scroll | Scroll                                                                |                
| FN+U                | Pause  | Pause                                                                 |
| &nbsp;              |        |                                                                       |
| FN+I                | Ins    | Insert (Vim-like and semantic binding)                                |
| FN+D                | Del    | Delete (semantic binding)                                             |
| FN+X                | Del    | Delete (Vim-like binding)                                             |
| FN+M                | Home   | Home                                                                  |
| FN+N                | End    | End                                                                   |
| FN+B                | PgUp   | Page Up (Vim-like binding)                                            |
| FN+F                | PgDn   | Page Down (Vim-like binding)                                          |
| &nbsp;              |        |                                                                       |
| FN+K                | Up     | Up (Vim-like binding)                                                 |
| FN+J                | Down   | Down (Vim-like binding)                                               |
| FN+H                | Left   | Left (Vim-like binding)                                               |
| FN+L                | Right  | Right (Vim-like binding)                                              |

Download the [Vim-like layout](layouts/vim-like-cidoo_qk61.layout.json) - use "Download as raw file".

### <a id="vim-like">Extended layout

This is an extended layout which extends the Vim-like layout with some navigation keys (including the arrow keys) in the 3rd layer.
To enter the 3rd layer the very bottom right key is used - let's call it the Raise (RS) key. I personally don't use this layout,
but I would like to share it because it might be useful for someone who misses the arrow keys and PgUp/PgDn keys are fun to use.

<p align="center">
<img alt="Layer 0" src="https://github.com/user-attachments/assets/2612d122-9666-4def-a8d4-31f79aad85d7" />
<img alt="Layer 2" src="https://github.com/user-attachments/assets/48d7c4ce-5bc4-4c70-b7e2-6828933d2061" />
<img alt="Layer 3" src="https://github.com/user-attachments/assets/061918d0-8dae-492a-ac22-a25d6a6792fc" />
</p>

| Key/Key combination | Key    | Description                                                           |
|---------------------|--------|-----------------------------------------------------------------------|
| FN+[                |        | Toggle LOGO LED light mode                                            |
| FN+]                |        | Toggle LOGO LED light color                                           |
| FN+Space            |        | Toggle ON/OFF Backlight                                               |
| FN+Backspace        |        | Reset the keyboard to the factory setting                             |
| &nbsp;              |        |                                                                       |
| -                   |        | Windows System (I don't need it)                                      |
| -                   |        | Mac System (I don't need it)                                          |
| &nbsp;              |        |
| CapsLock            | Esc    | Esc                                                                   |
| FN+Esc              | Esc    | Esc                                                                   |
| Esc                 | `      | Backtick                                                              |
| FN+1                | F1     | F1                                                                    |
| FN+2                | F2     | F2                                                                    |
| FN+3                | F3     | F3                                                                    |
| FN+4                | F4     | F4                                                                    |
| FN+5                | F5     | F5                                                                    |
| FN+6                | F6     | F6                                                                    |
| FN+7                | F7     | F7                                                                    |
| FN+8                | F8     | F8                                                                    |
| FN+9                | F9     | F9                                                                    |
| FN+0                | F10    | F10                                                                   |
| FN+-_               | F11    | F11                                                                   |
| FN+=+               | F12    | F12                                                                   |
| FN+T                | PrtSc  | Print Screen                                                          |
| FN+Y                | Scroll | Scroll                                                                |                
| FN+U                | Pause  | Pause                                                                 |
| &nbsp;              |        |
| FN+I                | Ins    | Insert (Vim-like and semantic binding)                                |
| FN+D                | Del    | Delete (semantic binding)                                             |
| FN+X                | Del    | Delete (Vim-like binding)                                             |
| FN+M                | Home   | Home                                                                  |
| FN+N                | End    | End                                                                   |
| FN+B                | PgUp   | Page Up (Vim-like binding)                                            |
| FN+F                | PgDn   | Page Down (Vim-like binding)                                          |
| &nbsp;              |        |
| FN+K                | Up     | Up (Vim-like binding)                                                 |
| FN+J                | Down   | Down (Vim-like binding)                                               |
| FN+H                | Left   | Left (Vim-like binding)                                               |
| FN+L                | Right  | Right (Vim-like binding)                                              |
| Extended keys       |        |
| RS+?/               | Up     | Up                                                                    |
| RS+FN               | Down   | Down                                                                  |
| RS+RAlt             | Left   | Left                                                                  |
| RS+RApp             | Right  | Right                                                                 |
| RS+<,               | Home   | Home                                                                  |
| RS+>.               | PgUp   | Page Up                                                               |
| RS+RShift           | PgDn   | Page Down                                                             |
| RS+M                | Mute   | Mute                                                                  |

Download the [extended layout](layouts/extended-cidoo_qk61.layout.json) - use "Download as raw file".
