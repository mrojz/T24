# Broken access control T24 Temenos

The attacker can modifiy the request POST parameter "enqname" to "HELPTEXT.MAINMENU" to list all available menus and save the menu id he want to choose.
Then modifiy the request POST parameter "enqname" to "USER". This will result in returning the full users list and the ability to view/edit them.
Then edit The menu to be displayed to current user by changing the input “Init Appln” ?X where X is the ID of the menu.
Logout and login again the new menu will be displayed
