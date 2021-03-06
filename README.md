# Clipboard History

ClipboardHistory is a <a href="http://www.microsoft.com/visualstudio/eng" target="_blank">Visual Studio</a>
extension that enables clipboard history.

It keeps track of all changes to the clipboard in a configurable list using a Tool Window.
You can then navigate the list to retrieve the desired clipboard data.

I developed this extension for my own needs, feel free to contribute if you can improve it.

## Supported Platforms

* Visual Studio 2012
* Visual Studio 2013
* Visual Studio 2015

## Release Notes
* [Version 2.0.0](/RELEASE-2.0.0.md)
* [Version 2.0.1](/RELEASE-2.0.1.md)

## Features

* Never lose code in the clipboard again!
* Simple Tool Window with a configurable Clipboard History List.
* Configurable clipboard events detection. (Global / Visual Studio instance).
* Duplicate entries prevention for the History List.
* Adaptable color scheme to fit with the selected theme in Visual Studio.
* Configurable ToolTip allows you to peek at the full clipboard item text.
* Double-Click on an item in the History List to put it back into the Clipboard. (v1.1+)

## Getting Started

* Download VSIX file from <a href="http://visualstudiogallery.msdn.microsoft.com/62040158-8ae2-4f87-8e09-0a3a812088ec" target="_blank">Visual Studio Extensions Gallery</a>.
* Install the extension using the vsix package and then **Restart Visual Studio**.
* Click **View** | **Other Windows** | **Clipboard History**.

| Picture | Description |
|---------|-------------|
| **Tool Window**<br>![ClipboardHistory Tool Window](/ClipboardHistory/AppResources/Images/ScreenShot_ToolWindow.png) | This tool window is the core of the Clipboard History extension. It keeps a list of past clipboard items ordered from the newest to the oldest.<br><br>To retrieve an item from the History List, simply Select this item and Press Ctrl + C. The item will be copied back into the Clipboard so that it can be Pasted (Ctrl + V) anywhere!<br><br>You can also change the extension's settings from that window. (See **Settings** section) |
| **MouseOver ToolTip**<br>![ClipboardHistory Tool Window](/ClipboardHistory/AppResources/Images/ScreenShot_ToolTip.png) | This ToolTip Window will display the Full Text contained in the Clipboard Item below the mouse cursor. It is configurable with a delay up to 99 seconds so it won't bother you if unwanted. |

## Settings

You can view and change the Settings of this extension by clicking on the "Settings" expander at the top of the ClipboardHistory Tool Window.
See more details on indivual settings below and also by putting your mouse over it in Visual Studio.
> *All Settings take effect immediately.*<br>
> *Invalid values will be ignored.*

| Picture | Description |
|---------|-------------|
| **Settings Panel**<br>![ClipboardHistory Settings Window](/ClipboardHistory/AppResources/Images/ScreenShot_Settings.png) | **History Max. Capacity**<br>Maximum number of items the history list can contain.  <br><br>**Lines Displayed per Item**<br>Maximum number of lines displayed for each item in the list.  <br><br>**ToolTip Hover Delay (in ms)**<br>Delay in milliseconds before the tooltip appears when you leave your mouse over an item in the list.  <br><br>**Visual Studio Clipboard Only**<br>Only track clipboard changes in the current Visual Studio instance.  <br><br>**Prevent Duplicate Items**<br>Ignores successive copy operations if the item data is the same as the last one.  <br><br>**Display Timestamp**<br>Display the Date and Time for each item. |

## Bug Tracker / Feature Request

Have a bug or a feature request? [Please open a new issue](https://github.com/kavengagne/ClipboardHistory/issues).

## License

ClipboardHistory is released under the [Apache License, Version 2.0](/LICENSE.txt).
