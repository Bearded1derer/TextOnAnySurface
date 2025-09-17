# Text on Any Surface Macro for FreeCAD

This macro for FreeCAD automates the process of adding multi-line text to a selected face of an object. It can project text onto standard surfaces and intelligently wrap text around annular (ring-shaped) faces.

It was created by Designify Labs with assistance from Gemini.

## ✨ Features

**Multi-Surface Support**: Works on both standard faces and annular (ring) faces.
**Curved Text Generation**: Automatically creates properly curved and wrapped text on ring-shaped surfaces.
**Auto-Scaling**: Intelligently scales the text to ensure it fits within the boundaries of the selected face.
**Flexible Operations**: Creates text as a `Raised` solid (Fuse/Union) or a `Cut` impression (Cutout) using robust boolean tools.
**Full Customization**: A user-friendly dialog box allows you to control:
    *Multi-line text input.
    *Any `.ttf` or `.otf` font file.
    *Font size, justification, and line spacing.
    *Thickness/Depth of the text solid.

## 📸 Screenshots

![Screenshot of the macro dialog box](https://github.com/Bearded1derer/TextOnAnySurface/blob/main/Dialog_Screenshot.png)
*The main user interface for text customization.*

![Screenshot of text on a flat or standard face](https://github.com/Bearded1derer/TextOnAnySurface/blob/main/Flat_Surface_Screenshot.png)
*Example of "Raised" text on a standard part.*

[![Screenshot of text on an annular face](https://github.com/Bearded1derer/TextOnAnySurface/blob/main/Annular_Surface_Screenshot.png)
*Example of "Cut" curved text on a ring.*

## ⚙️ Requirements

1.  A recent version of FreeCAD (v0.19 or newer).
2.  The **Curves Workbench**. This must be installed via the FreeCAD Addon Manager before running the macro.

## 💾 Installation

### Option 1: Recommended (via Addon Manager) Credit to TheMarkster from the freecad forums.

This method allows the macro to be updated easily through the Addon Manager.

1.  In FreeCAD, go to `Edit -> Preferences`.
2.  Select the `Addon Manager` section.
3.  On the "Custom repositories" tab, click the `+` button to add a new repository.
4.  Paste the following URL into the dialog:
    ```
    [https://github.com/Bearded1derer/TextOnAnySurface/](https://github.com/Bearded1derer/TextOnAnySurface/)
    ```
5.  Enter the following branch name:
    ```
    main
    ```
6.  Click "OK" and close the preferences window.
7.  Now, open the main Addon Manager via `Tools -> Addon Manager`. You should be able to find "TextOnAnySurface" in the "Macros" list to install or update it.

### Option 2: Manual Installation

1.  Download the `TextOnAnySurface.FCMacro` file from this repository.
2.  Find your FreeCAD macro directory by going to `Macro -> Macros...` and checking the "User macros location".
3.  Place the downloaded `.FCMacro` file into that directory.

## 🚀 Usage

1.  Open your model in FreeCAD.
2.  Select a single face on any solid object.
3.  Run this macro by going to `Macro -> Macros...`, selecting `TextOnAnySurface.FCMacro`, and clicking "Execute".
4.  Fill out the dialog with your desired text, font, and settings.
5.  Click "OK". The macro will create a new object with the text applied.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/Bearded1derer/TextOnAnySurface/blob/main/LICENSE) file for details.
