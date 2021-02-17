# autovpn2
![](https://img.shields.io/badge/autovpn2-python_2.7-blue.svg?style=flat-square) ![](https://img.shields.io/badge/dependencies-openvpn-orange.svg?style=flat-square)  [![](https://img.shields.io/badge/License-WTFPL%202.0-lightgrey.svg?style=flat-square)](http://www.wtfpl.net/) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=flat-square)](https://github.com/ruped24/autovpn2/graphs/commit-activity) [![HitCount](http://hits.dwyl.io/ruped24/ruped24/autovpn2.svg?style=flat-square)](http://hits.dwyl.io/ruped24/ruped24/autovpn2)

[VPN Gate](https://www.vpngate.net/en/) Client to Free VPN Access. You can get through firewalls and beyond to browse restricted websites. 

---

### Usage:

```bash
sudo autovpn2 JP
```

<details><summary>Expand for usage</summary>
<br>

**How to connect to a VPN Gate server:**

Use the [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2) list to get the country code. 

<details><summary>Expand for VPN Gate Servers List</summary>
<br>

[► **VPN Gate Servers List**](https://www.vpngate.net/en/)

</details>

_E.g._ Korea Republic (**KR** [:kr:](https://en.wikipedia.org/wiki/South_Korea))

To **start** the VPN: _E.g._ ` sudo autovpn2 KR`

To **stop** the VPN: Press <kbd>CTRL + c</kbd> 

The _autovpn2_ script will ask if you want to try another VPN.

If you want to retry another VPN, then press <kbd>y</kbd>, if you want to quit, press <kbd>n</kbd>


<details><summary>Expand for screenshot, demo and test</summary>
<br>
  
[▹ Check My IPx](https://ipx.ac/)

[▹ Anonymity check](http://proxydb.net/anon)

[▹ What is my proxy](http://www.whatismyproxy.com)

[▹ DNS leak test](https://www.doileak.com/classic.html)

:white_square_button: **|** [**Screenshot**](https://drive.google.com/file/d/10oEKydkW7YzZFK7VLOvAzz3HSzSIoED4/view?usp=sharing) **|** [**Demo**](https://drive.google.com/file/d/16VfJfKZqqR0RYzVxmPgfhGNKwsuYHVph/view?usp=sharing) **|**

</details>


</details>

---

### Dependencies:
```bash
apt install openvpn
```
---

### Installation:
```bash
sudo mv autovpn2.py /usr/local/bin/autovpn2
```
---

### Frequently Asked Questions:
<details><summary>Expand for Frequently Asked Questions</summary>

### FAQ:

> The default USA (**US** [:us:](https://en.wikipedia.org/wiki/United_States)) servers seems to be slow to me, which country is the fastest?
 
In "my" testing, Japan (**JP** [:jp:](https://en.wikipedia.org/wiki/Japan)) or Korea Republic (**KR** [:kr:](https://en.wikipedia.org/wiki/South_Korea)) servers seems to be "faster". 

> Can I change the default country code?

Yes, you can change the default [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2) standard code in the script.

Change Line [21](https://github.com/ruped24/autovpn2/blob/80782a993fafc99a2b8eb67861f15bf654cef594/autovpn2.py#L21) and 
Line [45](https://github.com/ruped24/autovpn2/blob/80782a993fafc99a2b8eb67861f15bf654cef594/autovpn2.py#L45) to the country code (Uppercase) of your choice.

> How to fix my DNS leak?

Pick one of these free and public [DNS](https://www.lifewire.com/free-and-public-dns-servers-2626062) Servers.

> This is a technical question, WHY Python 2.7???! It's [EOL](https://www.python.org/dev/peps/pep-0373/#maintenance-releases) dude! :confused:

Haha, The truth is, I didn't want to fight (_choosing my battles_;) with [Python3](https://www.pythonconverter.com/)'s bytes to string conversions for this [_one-off_](http://www.wtfpl.net) script.

Personally, I compile my legacy Python 2.7 standalone scripts to a Linux ELF 64-bit LSB executable using [Nuitka](https://nuitka.net/doc/user-manual.html) and [makeself](https://github.com/megastep/makeself#usage).  The created binary executes independent of a Python installation.

A [precompiled x86_64 autovpn2 binary](https://github.com/ruped24/autovpn2/releases/tag/v1.0) can be found under releases.

> What's with the name and the "2"?

I wrote this as a drop in replacement for the original [autovpn](https://en.kali.tools/?p=418) written in [Go](https://en.wikipedia.org/wiki/Go_(programming_language)), that's now in Github's [Digital Haven](https://github.com/adtac/autovpn).

The "2" is to not conflict with the original script if installed on said system. 

```diff
- Note: autovpn2 defaults to the US servers. The Japan (JP) servers are preferred.
```

</details>

---

#### Legal Disclaimer:

###### We are not affiliated with [VPN Gate](https://www.vpngate.net/en/) in any way. We are not advocating the use of their or any Free VPN service.

