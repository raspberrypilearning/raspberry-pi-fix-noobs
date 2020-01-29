## Break Raspbian
One day you might break your installation of Raspbian by accident. Perhaps you'll make changes to the configuration and not be able to get things back to the default. Perhaps you'll follow incorrect or out of date instructions on the internet and delete or break something important. Perhaps you'll install an incompatible application which stops something else working. Perhaps you'll run a command or script with a bug in it and delete or break something. 

Sometimes you'll understand what went wrong and be able to fix it. Sometimes it's better to just start again with a clean installation of Raspbian. 

You're now going to deliberately break your installation of Raspbian so you can see what it's like to fix it.

Raspbian uses the LXDE desktop environment to provide features such as the task bar and menus. An important part of LXDE is the panel. Let's delete the panel executable file (application). 

+ Open a terminal window from the task bar. 

+ Type the command

~~~
which lxdepanel
~~~

The output tells you where the lxdpanel executable file can be found. 

+ Move to the directory (folder) where this file is stored:

~~~
cd /usr/bin
~~~

+ The unix command for deleting a file is 'rm'. You can try deleting the file:

~~~
rm lxdepanel
~~~

but you won't be able to do it as the 'pi' user. 

+ Run the same command as a superuser:

~~~
sudo rm lxdepanel
~~~

+ Type the command

~~~
which lxdepanel
~~~

and you will see that the lxdepanel file has gone. 

This won't cause any immediate problems as the application is already running.

+ Reboot your Raspberry Pi by opening the main menu and choosing Shutdown and then the Restart option. 

+ When you Raspberry Pi reboots you should see something like this:

Oh dear. You've broken Raspbian. This time you've done it on purpose, but something like this might happen by accident in future. 


