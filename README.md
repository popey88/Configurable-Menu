Cinnamon Applet: Configurable Menu version v0.9-Beta
==============

Release Date: 28 january 2014

Authors: Lester Carballo Pérez(https://github.com/lestcape) and Garibaldo(https://github.com/Garibaldo).

Email: lestcape@gmail.com

Website: https://github.com/lestcape/Configurable-Menu

More Information: https://github.com/lestcape/Configurable-Menu/wiki

--------------

"Configurable Menu is a fork of the Cinnamon stock menu applet. It has much more features and is extremely configurable."

![Alt text](/configurableMenu@lestcape/Capture.png)

This latest version brings a lot of cool new stuff.

Be cautious: This applet is still considered non-stable and may have bugs... Install it for testing purposes only.

Some features:
--------------

1.	You choose how the menu should be opened: by pressing & releasing the mouse button, by just pressing the mouse button, or by hovering the mouse pointer on the menu icon.
2.	You can define the exact size of the menu (width and height) using the menu settings.

3.	Now you can also resize the menu by dragging a resize handle (on the menu corner) with the mouse!

4.	Now you can show the menu in full screen mode!

5.	You can choose among many different menu layouts.

6.	You can choose among many different system buttons layouts.

7.	The menu can show a magnified picture of the icon which is being hovered, similarly to the Windows 7 start menu.

8.	You can show/hide favorites, hover icon, system buttons, control buttons, data/time, separators etc...

9.	You can separate the system buttons from the favorites.

10.	You have two different modes of viewing the application entries: List View and Grid View.

11.	List View can have multiple columns.

12.	You can have favorites with multiple lines (rows or columns).

13.	You can drag & drop menu items onto the desktop.

14.	Autoscrolling works also horizontally when using some menu layouts.

15.	You can define the size of the application icons, category icons, favorites icons, system buttons, control buttons etc.

16.	You can define the font size of the application description/name.

17.	You can have a different configuration for each layout.

18.	The removable drives are now show in accessible panel and also can be removed directly.

19.	Now you can rename the apps on the accessible panel.

20.	And much more coming...


This program is free software:
--------------
You can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.


Installation Instructions:
--------------
1. Download this applet from their website : https://github.com/lestcape/Configurable-Menu
2. Unzip the downloaded file and copy the folder configurableMenu@lestcape at /home/USERNAME/.local/share/cinnamon/applets/ where USER is the user for your operating system.
3. Enable the applet in Cinnamon Settings and use it.

Add theme support:
--------------
- List of new style class and pseudo style class for the main menu box:
    - menu-main-box

- List of new style class and pseudo style class for the hover icon:
    - menu-hover-icon-box
    - menu-hover-icon-box:open

- List of new style class and pseudo style class for the control buttons:
    - menu-control-buttons-box
    - menu-control-resize-box
    - menu-control-view-box
    - menu-control-button
    - menu-control-button:open
    - menu-control-button-selected (when hover or focus)

- List of new style class and pseudo style class for the accessible panel:
    - menu-accessible-box
    - menu-accessible-devices-box
    - menu-accessible-places-box
    - menu-accessible-system-box

- List of new style class and pseudo style class for the Mint layout:
    - menu-operative-mint-box
    - menu-top-mint-box
    - menu-bottom-mint-box

- List of new style class and pseudo style class for the Windows 7 layout:
    - menu-operative-windows-box
    - menu-top-windows-box
    - menu-bottom-windows-box

- List of new style class and pseudo style class for all layouts except the Windows 7 and Mint layout:
    - menu-top-box
    - menu-bottom-box

- List of new style class and pseudo style class for the GnoMenu layouts (Note: The buttons can position in the future in 4 different ways, it's why we have 4 existing style classes):

    - menu-gno-button-box
    - menu-gno-operative-box
    - menu-gno-operative-box-selected (when hover or focus on any gno button)
    - menu-gno-button-left
    - menu-gno-button-left-selected (when hover or focus)
    - menu-gno-button-right
    - menu-gno-button-right-selected (when hover or focus)
    - menu-gno-button-top
    - menu-gno-button-top-selected (when hover or focus)
    - menu-gno-button-bottom
    - menu-gno-button-bottom-selected (when hover or focus)
    - menu-gno-power-left (just the parent of power panel, not the power panel)
    - menu-gno-power-right (just the parent of power panel, not the power panel)
    - menu-gno-power-top (just the parent of power panel, not the power panel)
    - menu-gno-power-bottom (just the parent of power panel, not the power panel)

- Settings restrictions on the style class:

    - menu-accessible-box:         Can only used if the option "Accessible panel has a box" it's active.
    - menu-accessible-devices-box: Can only show if you have any removable device.
    - menu-hover-icon-box:         Can only show if the option "Hover icon have a box" it's active.
    - menu-control-resize-box:     Can only show if the option "Control buttons have a box" it's active.
    - menu-control-view-box:       Can only show if the option "Control buttons have a box" it's active.
    - menu-gno-button-box:         Can only used if the option "GnoMenu buttons have a box" it's active.

More info: https://github.com/lestcape/Configurable-Menu/wiki/Add-theme-support

Add new languages:
--------------

1. Install the poedit program.
2. Open the file default.po with the poedit software. This file is located in the folder /home/USER/.local/share/cinnamon/applets/configurableMenu@lestcape/locale/
3. Make the translation, save the result, and send the .po file updated by the e-mail address here present, or add directly into the website of this software

More info: https://github.com/lestcape/Configurable-Menu/wiki/Add-new-languages

Change Log:
==============
0.9-Beta
   - Was added support for more languages.
   - Was added spanish language.
   - Now you can have a different configuration for each layout.
   - The removable drives are now show in accessible panel and also can be removed.
   - The full screen mode was improved, now can be see better in more themes.
   - Now the property "Maximum width of the application entry text" it's really a maximum width and not the width.
   - Added support for the old Clutter.Color API to fix the bug "Clutter.Color.from_string is not a function" when you start the applet.
   - Fixed the bug on mint and windows 7 layouts. This error involves the closure of the menu in the case of the searchEntry do not has a focus.
   - The Menu now can be improved using the css file of any Cinnamon theme.
   - Removed the hover icon borders, due to allow more compatibility with cinnamon themes.
   - The new layouts of Vampire, Garibaldo, GnoMenu Left, GnoMenu Right GnoMenu Top and GnoMenu Bottom was added.
   - Several visually improvement in different layouts, especially the horizontal.
   - Now you can rename the apps on the accessible panel.

0.8-Beta
   - The Accessible panel is now configurable and has two drag and drop areas (Places and Apps).
   - Implemented new “Places” fields (PC, Desktop, Home, Network and Trash).
   - You can add items to the accessible panel with a submenu and a drag and drop operation.
   - The favorites icons have now submenus.
   - Reduced the width of search item on windows 7 layout to be the same size or less of favorites area.
   - System buttons have now several layouts available.
   - The Accessible panel can have icons or not.
   - Categories can have icons or not.
   - You can remove the box pointer from the menu.
   - Implementation of separators, with configurable options.
   - The hover icon has a configurable border now.
   - Now you can align the menu to the screen edge.
   - When the menu is re-sizable, a resize handle appears on the corresponding corner.
   - Now you can expand the menu to full screen mode.
   - Now you can have the application description in the application entries.
   - Performance improvements.
   - Many bug fixes.

0.7-Beta
   - Fixed a bug in the keyboard navigation, and add for more componets.
   - Now you can control the size of all icons in the menu.
   - Added Accessible theme to allow the bar like Mint menu.
   - Added Accessible Inverted theme to allow the bar like Windows menu.
   - Added Mint theme.
   - Added Windows 7 theme.
   - A button to swap "all app" by "favorites" was implemented.
   - The favorites can show the text of applications also in icon and list view mode.
   - The power buttons was reimplemented, now are better.
   - The internal layout have change to support the new accessible bar.
   - Several minor bugs are fixed(but i know that have some more for example in Mint theme).
   - Added settings button.
   - Time and date now appear only when you don't have any app selected in the same place of title and description.
   - Time and date can be set visible or hide.
   - Now you can select if description and title of selected app appear, also you can change the font size.
   - Implementation of power buttons box to be modular.
   - Implementation of scroll buttons class to be modular, also now allow to handle the height so much better.
   - Changed the mode of controlling the numbers of columns of the items view.
   - Added option to resize the menu with the mouse.
   - Added button to the control box to allow or not the resize of menu.

0.6-Beta
   - Fixed several bugs.
   - Ability to drag and drop items to Desktop.
   - Now the option "add to panel" do not open panel launcher applet if it's closed.
   - Now the option "add to panel" also add item to icon list applet of physic if it's open.
   - Fixed the keyboard navegation.
   - Unified mechanisms for the different items views.
   - Show and hide power buttons.

0.5-Beta
   - Added Dragon theme to put the categories horizontally.
   - Added Horizontal theme to put  all horizontally.
   - Added Dragon Inverted theme to put the favorites in left.
   - Implementation of horizontal auto scrolling(do not exist in cinnamon).
   - Implementation of favorites with multiple lines.
   - Implementation of items multicolumn horizontal.

0.4-Beta
   - Fixed bug in list view mode that cause lag when you change categories.
   - Fixed bug in icon view mode when searching app.
   - Option "allow path entry in the menu search box", now work again and it's better.
   - Fixed some minors bugs.

0.3-Beta
   - Added view items.

0.2-Beta
   - Added functionality and menu on hover icon.

0.1-Beta
   - Initial release.

==============
To report bugs, request new features and make suggestions, please visit:
https://github.com/lestcape/Configurable-Menu/issues

You can also send us pull requests:
https://github.com/lestcape/Configurable-Menu/pulls

==============
Thank you very much for using this product.
Lester and Garibaldo.
