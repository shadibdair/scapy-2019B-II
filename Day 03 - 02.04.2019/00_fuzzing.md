# Using byobu
* install byobu with this command:
```bash
root@Secondary:~# sudo apt install byobu
```
* check what is byobu
```
root@Secondary:~# whatis byobu
byobu (1)            - wrapper script for seeding a user's byobu configuration and launching a text based window manager 
```
* use byobu
```bash
root@Secondary:~# byobu
```
* open a new window in byobo: press `control + a` and then press `c`
* go to the next window in byobo: press `control + a` and then press `n`
## Byobu keybindings
The common key bindings are:
```
       F2 - Create a new window

       F3 - Move to previous window

       F4 - Move to next window

       shift-F2 - Split the screen horizontally

       ctrl-F2 - Split the screen vertically

       shift-F3 - Shift the focus to the previous split region

       shift-F4 - Shift the focus to the next split region

       shift-F5 - Join all splits

       ctrl-F6 - Remove this split

```

### example of fuzzing usage : Browser security
Modern web browsers undergo extensive fuzzing. The Chromium code of Google Chrome is continuously fuzzed by the Chrome Security Team with 15,000 cores. For Microsoft Edge and Internet Explorer, Microsoft performed fuzzed testing with 670 machine-years during product development, generating more than 400 billion DOM manipulations from 1 billion HTML files.

* stress testing Vs fuzzing

# example 1:
* in order to dump traffic on a network, run in first window:
```
sudo tcpdump -i lo
```
* run in second window (with scapy):
```
send(IP(dst="127.0.0.1")/fuzz(TCP()),loop=1)
```
