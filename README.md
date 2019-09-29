# Sublime Indent and braces
Sublime text 2 & 3 plugin to indent selection and wrap it in braces. Useful to add if () statements for example.

![Alt text](http://fat.gfycat.com/HelpfulFittingCrownofthornsstarfish.gif)


## Installation

### By Package Control

1. Download & Install `Sublime Text 3` (https://www.sublimetext.com/3)
1. Go to the menu `Tools -> Install Package Control`, then,
   wait few seconds until the `Package Control` installation finishes
1. Go to the menu `Preferences -> Package Control`
1. Type `Package Control Add Channel` on the opened quick panel and press <kbd>Enter</kbd>
1. Then, input the following address and press <kbd>Enter</kbd>
   ```
   https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
   ```
1. Now, go again to the menu `Preferences -> Package Control`
1. This time type `Package Control Install Package` on the opened quick panel and press <kbd>Enter</kbd>
1. Then, search for `IndentAndBraces` and press <kbd>Enter</kbd>

See also:
1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.


1. Add the following shortcut to your keybindings (customize keys as desired)
````
{ "keys": ["ctrl+i"], "command": "indent_and_braces" },
````

Options
=======

__`opening_brace` & `closing_brace`:__ These options allow you to modify the kind of braces the plugin will insert.<br>

    { "keys": ["ctrl+shift+i"], "command": "indent_and_braces", "args": { "opening_brace": "[", "closing_brace": "]" } },

__`from_cursor`:__ Normally the plugin will determine intelligently wether or not to place the opening brace on a new line. If you want to force this, you can use `from_cursor`.<br>

    { "keys": ["ctrl+j"], "command": "indent_and_braces", "args": { "from_cursor": false} },
