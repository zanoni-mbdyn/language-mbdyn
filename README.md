# language-mbdyn
Syntax highlighting plugin for general purpose, free multibody analysis software [MBDyn](https://www.mbdyn.org/) input files.

## Features

 * Fully context-depending syntax highlighting
 * Autocompletion snippets for (almost) full input syntax

## Tips
By default, Atom assigns to the `Tab` key both the `snippets:next-tab-stop` and the `snippets:expand` commands. This leads to a rather clumsy way of navigating through snippets tab stops using nested snippets and standard Atom autocompletion. My suggestion is to change the binding of `snippets:next-tab-stop` and `snippets:previous-tab-stop`. 

Just as an example, my configuration in the `keymap.cson` file is
```
'atom-text-editor:not([mini])':
  'cmd-tab': 'snippets:next-tab-stop'
  'shift-tab': 'snippets:previous-tab-stop'
```

## Examples

Autocompletion at work in the definition of a structural node:

![strutural node autocompletion][autocompletion-node]
 
 [autocompletion-node]: http://github.com/zanoni-mbdyn/language-mbdyn/blob/master/docs/gifs/atom-mbdyn-node.gif
