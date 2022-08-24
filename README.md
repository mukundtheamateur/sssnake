# sssnake
The classic snake game for the terminal that can plays itself and be use like a screensaver.
[![asciicast](https://asciinema.org/a/477685.svg)](https://asciinema.org/a/477685)
## Installation

You need ncurses specifically ncursesw which is included in these packages:

```
apt install libncurses-dev       #Debian/Ubuntu/Mint
yum install ncurses-devel        #RHEL/CentOS/Fedora and Rocky Linux/AlmaLinux
pacman -S ncurses                #Arch Linux
zypper install ncurses-devel     #OpenSUSE 
xbps-install -S ncurses-devel    #Void linux
```

With that you can just do:


```
make
make install
```


## Usage

(The options are different than the options on the released versions. If you installed this program from the released page please check "sssnake -h")

By default it will run like a normal snake game that you can control with wasd, hjkl(vi keys) or the arrow keys.
But try this

```
sssnake -m screensaver -s 15
```

or

```
sssnake -l full -m screensaver -s 15 -j 5

```
press Q to quit.

Use the -h options to see the option details.

## Faq

- Does the snake fills the entire screen/terminal with the autopilot?
  No, at least not for now. I have plans to make the snake unkillable but unlike the current solution this will be resource intensive so it will have to be optional and not default.
- Why the name "sssnake"?
   All the snake games in the terminal that I found use ascii characters and lets be honest, they are kinda ugly. 
   I try to do something more visually appealing, something "sexy" and it can play itself so it is "smart". 
   Smart and sexy snake => sssnake.
- Why C?
  I like simple and efficient things.



## Credits

- Min heap implementation base on Martin Broadhurst min-heap ( http://www.martinbroadhurst.com/min-heap-in-c.html ) 
- A\* base on (https://www.geeksforgeeks.org/a-search-algorithm/)
