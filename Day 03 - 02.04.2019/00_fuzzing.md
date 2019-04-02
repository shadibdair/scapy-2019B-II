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
