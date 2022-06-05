# Extended String Property Editor

## Description

This enhanced property editor has been designed to get round two limitations of the standard Delphi string property editor.

1. The standard property editor does not allow multi-line strings with embedded CR/LF characters to be entered via the object inspector. Such strings can only be assigned at run-time.
2. Although long Delphi strings have a 2Gb size limit, the standard property editor only accepts strings up to 255 characters long. Once again, longer strings must be assigned at run-time.

The property editor works with all properties of type **string** or _TCaption_ of all components. It adds an ellipsis button to the right hand side of the data entry area in the object inspector. Clicking this button displays a dialogue box in which the property's value can be entered. Pressing return in the dialogue box starts a new line. There is no practical limit to the length of strings that can be entered.

Clicking _OK_ (or pressing Ctrl+Return) causes the entered text to be assigned to the property. If, or how, any newline characters will be displayed in the object inspector depends on the version of Delphi being used.

The edit dialogue is resizeable. Word wrapping can be switched on or off. Both the word-wrapping and dialogue box size and position are persistent. The dialogue box has a toolbar that provides buttons to:

* Select all the text in the editor.
* Clear all the text from the editor.
* Overwrite the editor's existing text with text from the clipboard.
* Copy all the text from the editor to the clipboard.
* Undo the last edit.
* Load text into the editor from a file.
* Save the contents of the editor to a file.
* Display online help.

In addition the normal cut, copy and paste operations are available via a context menu and the usual keyboard short-cuts.

## Compatibility

The property editor is reported to compile and work with all versions of Delphi from Delphi 6 onwards, except the .NET versions.

## Installation

The _Extended String Property Editor_ is supplied in a zip file. Before installing you need to extract all the files from the zip file. The following files will be extracted:

* **`PJStringPE.pas`** – Property editor source code.
* **`PJStringPE.dfm`** – Property editor form file.
* `README.md` – This read-me file.
* `CHANGELOG.md` – Change log.
* `MPL-2.txt` – Mozilla Public License v2.0.
* `DocumentationWiki.URL` – Internet short-cut to online property editor documentation.

`PJStringPE.pas` and `PJStringPE.dfm` must be included in a design time package that is then installed into the IDE. If you need help doing this [see here](https://delphidabbler.com/url/install-comp).

> **Note:** you must ensure the package containing the property editor includes the _DesignIDE_ package in its **requires** clause.

## Update History

A complete change log is provided in [`CHANGELOG.md`](https://github.com/ddablib/stringpe/blob/main/CHANGELOG.md) that is included in the download.

## License and Credits

These components are released under the terms of the [Mozilla Public License v2.0](https://www.mozilla.org/MPL/2.0/).

Thanks to the following who have contributed to this project:

* Richard C Haven
* Bino

All relevant trademarks are acknowledged.

## Acknowledgements

The property editor uses or adapts icons from the following collections:

* The 16×16 Free Application Icons packs by [Aha-soft](http://www.aha-soft.com/), licensed under a Creative Commons Attribution-Share Alike 3.0 license.
* The Free Pixelbox icon sets from [Icojam](https://www.icojam.com/), free to use in any kind of commercial or non-commercial project.

## Bugs and Feature Requests

Bugs can be reported or new features requested via the project's [Issue Tracker](https://github.com/ddablib/stringpe/issues). A GitHub account is required.

Please check if an issue has already been created for a similar report or request. If so then please add a comment containing as much information as you can to the existing issue, or if you've nothing to add, just add a :+1: (`:+1:`) comment. If there is no suitable existing issue then please add a new issue and give as much information as possible.

## About the Author

I'm Peter Johnson – a hobbyist programmer living in Ceredigion in West Wales, UK, writing mainly in Delphi. My programs and other library code are available from: [https://delphidabbler.com/](https://delphidabbler.com/).

This document is copyright © 2005-2022, [P D Johnson](https://gravatar.com/delphidabbler).
