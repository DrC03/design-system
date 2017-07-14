---
layout: page
title: Menus
category: elements
tags:
  - right
  - click
  - pull
  - cascading
  - application
  - bar
status: WIP
---
## Application menu

**Codename:** `ApplicationMenu` - NationalInstruments.Controls  
**Codename:** `ApplicationMenuItem` - NationalInstruments.Controls


## Context menus
**Codename:** `ShellContextMenu` - NationalInstruments.Controls.Shell

## Using icons in menus
In general, we do not use icons in context or application menus but there are a few exceptions.
 
#### Exceptions  
1. We do provide icons for file types and folders in the "New" menus
1. Run, Pause, Abort in LabVIEW.
The NI product you are working may have similar types of commands where it is also appropriate to use icons.
1. We do provide icons for items that are standard and well known in general computing. The specific items that meet that criteria are as follows:
  - Cut
  - Copy
  - Paste
  - Save
  - Save all
  - Print
  - Undo 
  - Redo
 
**Note:** We have excluded "Close" due to multiple versions of Close that exists in LabVIEW (Close, Close all, Close project, etc.) However, if your product has a simpler Close command, you may want to consider including that one, as well.

## Access keys for menus
Note: These guidelines do not cover access keys for dialog boxes or configuration panes.

**What’s the difference between an access key and a shortcut key?**

Shortcut keys are keys or combination of keys used by advanced users to perform frequently used commands for efficiency.
Access keys are keys or combination of keys used for accessibility to interact with menu items using the keyboard. Windows indicates access keys by underlining the access key. Windows hides access key underlines by default and shows them only when you press the Alt key. Unlike shortcut keys, access keys are not meant to be memorized.

**Assigning access keys**
Assign access keys to all menu items.

- For dynamic menu items, such as recently opened files, assign access keys numerically.
Access keys must be unique within the same menu level. You can reuse access keys across different menu levels. For Windows applications, there are standard access keys used for command commands listed [here](https://msdn.microsoft.com/en-us/library/windows/desktop/dn742465(v=vs.85).aspx#accesskeytable). Depending on the other access keys in the menu, you might not be able to use the standard assignment but check here first (especially if it’s a standard command).
Access keys should be easy to find:
- Characters with wide widths are preferred, such as w, m, and capital letters.
- For the most frequently used items, choose characters that are at the beginning of the first or second word, preferably the first character.
- For less frequently used menu items, choose letters with a distinctive consonant or vowel.
Avoid characters that make the underline difficult to see, such as characters that:
- Are only one pixel wide, such as I, i, L.
- Contain a descender, such as g, j, p, q, and y.
- Are next to a character with a descender.