PS: Arch Linux, Netrunner, Manjaro and other Arch-based distros can use the repo: 
http://download.tuxfamily.org/gericom/README.html

then hit: "sudo pacman -S screenfetch-netrunner" without the quotes.

It takes around 10 minutes, after update, to be uploaded. Thanks.

If you like my work, hit the DONATE button and send me a beer. Thank You!

https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=AVFTJ4N9M9AE2

# screenFetch - The Bash Screenshot Information Tool

## What is screenFetch?

screenFetch is a "Bash Screenshot Information Tool". This handy Bash
script can be used to generate one of those nifty terminal theme
information + ASCII distribution logos you see in everyone's screenshots
nowadays. It will auto-detect your distribution and display an ASCII
version of that distribution's logo and some valuable information to the
right. There are options to specify no ASCII art, colors, taking a
screenshot upon displaying info, and even customizing the screenshot
command! This script is very easy to add to and can easily be extended.

## How do I get screenFetch?

### Netrunner Rolling

1. Install `screenfetch-netrunner` from the official repositories. That's it!

### Arch Linux

1. Install `screenfetch` from the official repositories or `screenfetch-git` from the AUR. That's it!

### Mageia

1. Install screenfetch from the official repositories with urpmi or rpmdrake.
   e.g.: `urpmi screenfetch`

### Mac

1. Run `brew install screenfetch` after installing [Homebrew](http://brew.sh)

### Gentoo or Sabayon

1. Emerge screenfetch from portage using `emerge screenfetch`
2. Sabayon users can install screenfetch from entropy using `equo install screenfetch`

### Ubuntu (>14.04) and Debian (stable/testing/unstable)

1. Install: `apt-get install screenfetch`
2. There is also a PPA for Ubuntu located at https://launchpad.net/%7Edjcj/+archive/ubuntu/screenfetch

### FreeBSD

Install screenfetch using the [ports](https://freshports.org/sysutils/screenfetch/) system: `cd /usr/ports/sysutils/screenfetch/ && make install clean`
Install screenfetch as a binary package: `pkg install screenFetch`
If screenfetch doesn't work as expected, try to (re-)install bash: `cd /usr/ports/shells/bash/ && make install clean` or `pkg install bash`

### Fedora (21 or later)

1. Install it with yum running: `yum install screenfetch`

### Others

1. Download the latest source at https://github.com/KittyKatt/screenFetch
2. In a terminal, make the file executable by doing the following: `chmod +x /path/to/screenfetch/screenfetch-dev`
3. Then, either keep it there, or move it to somewhere in your $PATH to make it available without having to use the full path to the script.


## Running screenfetch

To run screenFetch, open a terminal of some sort and type in the command `screenfetch`
or wherever you saved the script to. This will generate an ASCII logo with the
information printed to the side of the logo. There are some options that may be
specified on the command line, and those are shown below or by executing `screenfetch -h`:

      -v                 Verbose output.
      -o 'OPTIONS'       Allows for setting script variables on the
                         command line. Must be in the following format...
                         'OPTION1="OPTIONARG1";OPTION2="OPTIONARG2"'
      -n                 Do not display ASCII distribution logo.
      -N                 Strip all color from output.
      -t                 Truncate output based on terminal width (Experimental!).
      -p                 Output in portrait mode, with logo above info.
      -s(m)              Using this flag tells the script that you want it
                         to take a screenshot. Use the -m flag if you would like
                         to move it to a new location afterwards.
      -c string          You may change the outputted colors with -c. The format is
                         as follows: [0-9][0-9],[0-9][0-9]. The first argument controls the
                         ASCII logo colors and the label colors. The second argument
                         controls the colors of the information found. One argument may be
                         used without the other.
      -a 'PATH'          You can specify a custom ASCII art by passing the path
                         to a Bash script, defining `startline` and `fulloutput`
                         variables, and optionally `labelcolor` and `textcolor`.
                         See the `asciiText` function in the source code for more
                         informations on the variables format.
      -S 'COMMAND'       Here you can specify a custom screenshot command for
                         the script to execute. Surrounding quotes are required.
      -D 'DISTRO'        Here you can specify your distribution for the script
                         to use. Surrounding quotes are required.
      -A 'DISTRO'        Here you can specify the distribution art that you want
                         displayed. This is for when you want your distro
                         detected but want to display a different logo.
      -E                 Suppress output of errors.
      -V, --version      Display current script version.
      -h, --help         Display this help.

## Contact Me

If you would like to suggest something new, inform me of an issue in the
script, become part of the project, or talk to me about anything else,
you can either email me at `gericom.hummer@gmail.com` or hangouts.
