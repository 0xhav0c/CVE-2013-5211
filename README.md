# CVE-2013-5211 PoC
## Network Time Protocol Daemon (ntpd) monlist Command Enabled DoS

This Python script is used to detect CVE-2013-5211, a vulnerability found in NTP (Network Time Protocol) servers. Using the ntpd monlist command, this vulnerability could allow an attacker to send a series of UDP packets to the server, consuming the server's resources.

The script sends a UDP packet to a user-specified NTP server and waits for a response from the server. If the server responds, the script indicates that it has the CVE-2013-5211 vulnerability. Otherwise, it is indicated that the server does not have this vulnerability.

```console
python3 CVE-2013-5211.py 192.168.x.x
```
