<p align="center">
  <img src="https://imgur.com/KEvaVTP.jpg" width="250px"></img>
</p>
<p align="center">
  <em>Inspired by</em>
  <a href="https://github.com/cknadler/vim-anywhere">cknadler/vim-anywhere</a>
</p>

<p align="center">
  <img src="https://thumbs.gfycat.com/PlumpDeadlyAlpinegoat-size_restricted.gif" width="500px"></img>
  <h2>What it does</h2>
  A keyboard shortcut of your choosing creates a temporary frame and buffer. The text is automatically inserted into the application you&apos;re using. Bust your moves on the fly, with fewer keystrokes. Invoke the shortcut with selected text and it will be replaced.
</p>

Note that this is a fork of [emacs_anywhere](https://github.com/zachcurry/emacs-anywhere) but with a better support for Linux. [See Faq](#faq) for more details.

## Install ##
### OSX ###
``` bash
curl -fsSL https://raw.github.com/psibi/emacs-everywhere/master/install | bash
```
Open **System Preferences** and navigate to **keyboard > shortcuts > Services**. Check the box beside "Emacs Everywhere" and click "Add Shortcut" and key a shortcut.

### Linux ###
>### dependencies: **xdotool** ###
>Install as needed
>``` bash
>sudo apt-get install xdotool

#### Installation ####


``` bash
curl -fsSL https://raw.github.com/psibi/emacs-everywhere/master/install | bash
```
Create a keyboard shortcut with this command `$HOME/.emacs_everywhere/bin/run`

### Windows ###
TBD

## How to ##
Invoke the shortcut. A new frame will be created and display an empty buffer titled `*Emacs Everywhere*`. When the frame is deleted the buffer's content is inserted into the application you're using and the buffer is deleted. Any text selected when the keyboard shortcut is invoked will be replaced.

## Update ##
``` bash
~/.emacs_everywhere/update
```

## Uninstall ##
``` bash
~/.emacs_everywhere/uninstall
```

## Slow? ##
If your Emacs server isn't running when you use the keyboard shortcut, **Emacs Everywhere** will start it (this is slower). Run Emacs as a daemon (`emacs --daemon`) to start your server from the command line, or use `server-start` command in Emacs. Once you've a got a running server, new frames are created much faster.

## TODO ##
- Emacs command to toggle **Emacs Everywhere**
- Homebrew
- Windows

## FAQ

### Why the fork ? 

Because the orignal maintainer didn't want to a non clipboard based approach for Linux systems. See these issues for more details:
* [PR 23](https://github.com/zachcurry/emacs-anywhere/pull/23)
* [Issue 18](https://github.com/zachcurry/emacs-anywhere/issues/18#issuecomment-370259456)
* [Issue 36](https://github.com/zachcurry/emacs-anywhere/issues/36)


## Contributing ##
All contributions and pull requests are welcome.

Copyright © 2018, Sibi Prabakaran & Zach Curry, All rights reserved.
