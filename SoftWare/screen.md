---
title: Screen 速查表
toc: true
tags:
  - Screen
date: 2009-01-01 21:40:52
updated: 2009-01-01 21:40:52
categories:
  - software
---
# Screen 速查表

## Screen

```bash
   _____
  / ___/_____________  ___  ____
  \__ \/ ___/ ___/ _ \/ _ \/ __ \
 ___/ / /__/ /  /  __/  __/ / / /
/____/\___/_/   \___/\___/_/ /_/

```

Quick install:

1. Screen
login as root:
sudo su -
yum -y install screen

2. start screen
  screen

3. create a new screen
CTRL-A  c

4. go to next screen
CTRL-A n,   CTRL-A p

5. detatch from a screen
 CTRL-A d

6. reattach to screen
sceen -r

7. list screen
screen -list

8. Log
CTRL-A H

9. look for activity
"Ctrl-a" "M"

10. look for in activity
"Ctrl-a" "_"

### Screen -Help

```bash
Options:
-a            Force all capabilities into each window's termcap.
-A -[r|R]     Adapt all windows to the new display width & height.
-c file       Read configuration file instead of '.screenrc'.
-d (-r)       Detach the elsewhere running screen (and reattach here).
-dmS name     Start as daemon: Screen session in detached mode.
-D (-r)       Detach and logout remote (and reattach here).
-D -RR        Do whatever is needed to get a screen session.
-e xy         Change command characters.
-f            Flow control on, -fn = off, -fa = auto.
-h lines      Set the size of the scrollback history buffer.
-i            Interrupt output sooner when flow control is on.
-l            Login mode on (update /var/run/utmp), -ln = off.
-list         or -ls. Do nothing, just list our SockDir.
-L            Turn on output logging.
-m            ignore $STY variable, do create a new screen session.
-O            Choose optimal output rather than exact vt100 emulation.
-p window     Preselect the named window if it exists.
-q            Quiet startup. Exits with non-zero return code if unsuccessful.
-r            Reattach to a detached screen process.
-R            Reattach if possible, otherwise start a new session.
-s shell      Shell to execute rather than $SHELL.
-S sockname   Name this session <pid>.sockname instead of <pid>.<tty>.<host>.
-t title      Set title. (window's name).
-T term       Use term as $TERM for windows, rather than "screen".
-U            Tell screen to use UTF-8 encoding.
-v            Print "Screen version 4.00.02 (FAU) 5-Dec-03".
-wipe         Do nothing, just clean up SockDir.
-x            Attach to a not detached screen. (Multi display mode).
-X            Execute <cmd> as a screen command in the specified session.
```

```bash
Basic
=====
    ctrl a c              -> cre­ate new win­dow
    ctrl a A              -> set win­dow name
    ctrl a w              -> show all win­dow
    ctrl a 1|2|3|…        -> switch to win­dow n
    ctrl a ”              -> choose win­dow
    ctrl a ctrl a         -> switch between win­dow
    ctrl a d              -> detach win­dow
    ctrl a ?              -> help
    ctrl a [              -> start copy, move cur­sor to the copy
                             loca­tion, press ENTER, select the chars,
                             press ENTER to copy the selected
                             char­ac­ters to the buffer
    ctrl a ]              -> paste from buffer


How to start screen
===================
    screen –DR            -> list of detached screen
    screen –r PID         -> attach detached screen ses­sion
    screen –dmS MySes­sion -> start a detached screen ses­sion
    screen –r MySes­sion   -> attach screen ses­sion with name MySession


Advanced
========
    ctrl a S              -> cre­ate split screen
    ctrl a TAB            -> switch between split screens

    ctrl a Q              -> Kill all regions but the cur­rent one.
    ctrl a X              -> remove active win­dow from split screen
    ctrl a O              -> logout active win­dow (dis­able out­put)
    ctrl a I              -> login active win­dow (enable output)
```
