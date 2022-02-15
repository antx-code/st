Antx's bulid of st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.

Requirements
------------
In order to build st you need the Xlib header files.

Installation
------------
If you are in Manjaro or any arch linux envirement, you should install st first with yay, which like below:

    yay -S st

Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

If you want to use my st fonts, you can download nerd-fonts with yay like below:

    yay -S nerd-fonts-source-code-pro 

or

    yay -S nerd-fonts-mononoki

Afterwards enter the following command to build and install st (if
necessary as root):

    sudo make clean install

Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

