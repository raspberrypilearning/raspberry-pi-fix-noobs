## Shutdown Raspbian

You need to shutdown Raspbian and restart it to be able to enter NOOBS and restore your system. How can you shutdown Raspbian without the menu!

+ You can shut Raspbian down from the command line but to do this you'll need a terminal window to type the command in. You can't open the terminal from the main menu or from the task bar without the LXDE panel. Fortunately there's a keyboard shortcut for opening a terminal window. Type Ctrl-Alt-T, that is hold down the Ctrl and Alt keys and tap T. 

+ In the terminal window that opens, type the following command:

~~~
shutdown -r now
~~~

This will shutdown your Raspberry Pi. The `-r` option tells it to restart and 'now' says to do it immediately. 


In our situation we were still able to use Raspbian and shut it down cleanly. If you end up in a real situation where these options aren't working and you have ssh enabled then you may be able to log in remotely and run the `shutdown -r now` command to restart the computer and access NOOBS. See [Raspberry Pi ssh documentation](https://www.raspberrypi.org/documentation/remote-access/ssh/) for more details.

+ If you end up in a situation where none of the options for cleanly shutting down Raspbian are working then you will have to just power off Raspbian. This is not an option you should choose if you can avoid it as you risk damaging your SDCard and losing data. 
