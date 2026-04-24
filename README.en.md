## :: Overview ::

This is a custom layout definition file for [Onboard](https://github.com/onboard-osk/onboard), the on-screen keyboard.
It replicates the layout of a Japanese keyboard (compliant with OADG109A/JIS X 4064).

This file was created by copying the official `/usr/share/onboard/layouts/Full Keyboard*` files and customizing them.
You can check which parts have been modified by comparing the differences between these files.

```console:Example:
    $ diff layouts/OADG109A_Full_Keyboard.onboard /usr/share/onboard/layouts/Full\ Keyboard.onboard
```

You will need a Linux desktop environment with a Japanese environment setup. maybe.


## :: Installation Instructions ::

Please clone this repository using the `git clone` command.
This will create the `layout` directory; simply place it in an XDG-compliant directory that Onboard can recognize.
You can install it in your home directory using the following commands:

```console:
    $ mkdir OADG109A_Full_Keyboard && cd OADG109A_Full_Keyboard
    $ git clone https://github.com/9hnder/OADG109A_Full_Keyboard
    $ mkdir -p ~/.local/share/onboard/
    $ cp -r OADG109A_Full_Keyboard/layout  ~/.local/share/onboard/
```

The `theme` directory is optional. Use the design if you need it.


## :: How to Use ::

After installation, if Onboard is already running, close it and restart it.
Then, open the Onboard settings screen and select *[Layout] > [My Layouts] > [OADG109A_Full_Keyboard]*.

To try it from the CLI:

```console:
    $ pkill onboard
    $ onboard-settings
    -- (Set “OADG109A_Full_Keyboard” layout) --
    $ onboard &
```

Let's do this!


## :: License ::

Following the original project, the license is as follows. Modification and redistribution are permitted as long as the license terms are adhered to.

[GPL-3+](https://www.gnu.org/licenses/gpl.txt)


© Ken Shirakawa (9hnder)
Since: 2026-04-18 - 2026-04-23


## :: Disclaimer ::

The author assumes no responsibility for any issues that may arise from using these settings.
Please use at your own risk.


## :: Test Environment ::

The author’s test environment is as follows. It is a physical machine, not a virtual environment... maybe.
(Unless this world is a simulator...)
This is the result of the `neofetch` command.

             ...-:::::-...                 9hnder@SilverSurfer
          .-MMMMMMMMMMMMMMM-.              -------------------
      .-MMMM`..-:::::::-..`MMMM-.          OS: Linux Mint 22.3 x86_64
    .:MMMM.:MMMMMMMMMMMMMMM:.MMMM:.        Host: Surface Go 1
   -MMM-M---MMMMMMMMMMMMMMMMMMM.MMM-       Kernel: 6.17.0-19-generic
 `:MMM:MM`  :MMMM:....::-...-MMMM:MMM:`    Uptime: 7 days, 27 mins
 :MMM:MMM`  :MM:`  ``    ``  `:MMM:MMM:    Packages: 2143 (dpkg)
.MMM.MMMM`  :MM.  -MM.  .MM-  `MMMM.MMM.   Shell: bash 5.2.21
:MMM:MMMM`  :MM.  -MM-  .MM:  `MMMM-MMM:   Resolution: 2400x1600
:MMM:MMMM`  :MM.  -MM-  .MM:  `MMMM:MMM:   DE: Cinnamon 6.6.7
:MMM:MMMM`  :MM.  -MM-  .MM:  `MMMM-MMM:   WM: Mutter (Muffin)
.MMM.MMMM`  :MM:--:MM:--:MM:  `MMMM.MMM.   WM Theme: Mint-Y-Dark-Red (Mint-Y)
 :MMM:MMM-  `-MMMMMMMMMMMM-`  -MMM-MMM:    Theme: Mint-Y-Dark-Red [GTK2/3]
  :MMM:MMM:`                `:MMM:MMM:     Icons: Mint-Y-Red [GTK2/3]
   .MMM.MMMM:-------- ------:MMMM.MMM.     Terminal: gnome-terminal
     ‘-MMMM.-MMMMMMMMMMMMMMM-.MMMM-’     CPU: Intel Pentium 4415Y (4) @ 1.600GHz
       '.-MMMM``--:::::--``MMMM-.'         GPU: Intel HD Graphics 615
            ‘-MMMMMMMMMMMMM-’            Memory: 7282MiB / 7818MiB
               ``-:::::-``


## :: References ::

I referred to the following web pages while creating this. Thank you.

[Bochibochi Blog](https://mypace.sasapurin.com/entry/impossible-input-underscore-onboard/)

Also, if you want to change the font on the keycaps or modify the Super key label, the following page will be helpful.

[kledgeb](https://kledgeb.blogspot.com/2014/06/ubuntu-onboard-17.html)


## :: About the Author ::

I’m basically a damning, but every now and then I switch to “serious mode” to write technical articles or create tools. You can find them here:

[GitHub](https://github.com/9hnder/)
[Qiita User Page](https://qiita.com/9hnder/)

Most of my articles are written with the goal of contributing to the spread of Linux. They are all Linux-related.
I planing to add a story about the creation of this configuration file at a later date.
Please check them out if you’re interested.

**Sorry, dear foreign friends! Only Japanese articles. DW.**


## :: Acknowledgments ::

I would like to thank the reference sites and the Onboard developers.
Thank you for the SUPER wonderful software!



# vim:set ts=4 tw=0 ff=unix ft=markdown : This is vim modeline #

