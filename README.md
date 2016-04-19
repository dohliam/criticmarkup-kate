# criticmarkup-kate - A CriticMarkup syntax highlighter for Kate editor/KatePart

The XML file in this repository (`criticmarkup.xml`) contains rules for highlighting [CriticMarkup](http://criticmarkup.com/) syntax in Markdown files in [Kate](http://kate-editor.org/), the default text editor for [KDE](https://www.kde.org/).

Once [installed](#installation), opening any file with the `.cmu` or `.critic` extension should automatically highlight CriticMarkup syntax as in the example below:

![CriticMarkup syntax highlighting screenshot](https://cloud.githubusercontent.com/assets/9295750/14648308/8613e108-0616-11e6-95ae-789f5e9cdaf6.png)

You can also manually select CriticMarkup syntax from the `Tools > Highlighting` menu in any normal Markdown file.

This highlighter works fine with Kate or [Kwrite](https://www.kde.org/applications/utilities/kwrite/) (which are both based on [KatePart](http://kate-editor.org/about-katepart/)), and should also work with most of the common features of both CriticMarkup and Markdown.

## Installation

Steps to install the CriticMarkup syntax highlighting file:

1. Download the file `criticmarkup.xml` or clone this repository
2. Find the folder `~/.kde/share/apps/katepart/syntax/` on your system (create it if it does not already exist)
3. Move `criticmarkup.xml` into `~/.kde/share/apps/katepart/syntax/`
4. Open or restart Kate to use the syntax highlighter.

Default syntax highlighting files for Kate are usually stored in the folder `/usr/share/kde4/apps/katepart/syntax/`. However, custom syntax highlighters should probably be saved in the local syntax highlighting folder (`~/.kde/share/apps/katepart/syntax/`) in the user's home directory so that they don't get accidentally overwritten during an update.

NOTE: The above applies to KDE 4. If you are using Plasma 5, the local folder for Kate syntax files has changed to `~/.local/share/katepart5/syntax/`.

## Usage

Files with the extension `.cmu` or `.critic` will automatically be highlighted using the rules in `criticmarkup.xml`. Plain text or other files can be forced to use CriticMarkup highlighting rules by selecting _CriticMarkup_ from the _Highlighting_ menu:

* __Tools__ > __Highlighting__ > __Markup__ > __CriticMarkup__

## Other Kate syntax highlighters

* [AsciiDoc / AsciiDoctor](https://github.com/dohliam/asciidoc-kate)
* [PmWiki](https://github.com/dohliam/pmwiki-kate)

## License
Based on [kate-markdown](http://github.com/claes/kate-markdown/) by [Claes Holmerson](http://github.com/claes/).

Inspired by [CriticMarkup for Emacs](https://github.com/joostkremers/criticmarkup-emacs) by [@joostkremers](https://github.com/joostkremers).

Dual-Licensed under both GPL and BSD licenses.
