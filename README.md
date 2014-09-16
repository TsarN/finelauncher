finelauncher
============

FineLauncher is an eye-candy launcher for linux based on mylaunchpad

Eyecandy Full Screen launcher script for openbox and other stand-alone window managers.

Run with python and gtk/cairo

Autor: Tsarev Nikita, Gabriel Sabillon

Credits:
  Based on MyLaunchpad

Original credits:
  Based in oblogout interface code by Andrew Williams and Archbang script for openbox pipe menu


*Dependences:
  *python-gmenu
  *pygtk
  *cairo
  *lxml

How to RUN:
  make the file finelauncher.py executable and run it

 	 $./finelauncher.py default

  or simply:
	
	 $./finelauncher.py


  By default the app works with xdg-menu  «applications.menu» of gnome-menus
  You can link another xdg-menu for example lxde-menu with ln command:

    $sudo ln -s /etc/xdg/menus/lxde-applications.menu /etc/xdg/menus/applications.menu

  Or You can change the default menu with your favorite xdg-menu like xfce-applications or lxde-aplications
  just send another xdg-menu like a argument simple run:
  
    $finelauncher.py lxde-applications



How to add launcher to panel(tint2):
 You can add this launcher in your tint2 panel creating a .desktop  file 
 
Desktop file example:
 
[Desktop Entry]
Type=Application
Name=Menu
Comment=Menu
GenericName=Menu
Icon= <<Insert your icon path here>>
Exec= <<Insert script path here>>
If your panel is tint2 you only need add a line in your config file:

launcher_item_app = /home/<<user>>/<<path>>/menu.desktop 

