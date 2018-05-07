# RCE on GPON home routers (CVE-2018-10561)

## Vulnerability
Many routers today use GPON internet, and  a way to bypass all authentication on the devices (**CVE-2018-10561**) was found by [VPNMentor](https://www.vpnmentor.com/blog/critical-vulnerability-gpon-router/). With this authentication bypass, it's also possible to unveil another command injection vulnerability (**CVE-2018-10562**) and execute commands on the device.

At the time it was written almost ONE MILLION of these devices are exposed to the Internet, according to [Shodan](https://www.shodan.io/search?query=title%3A%22GPON+Home+Gateway%22).


## Dependencies required
`request`

`urllib2`

## Tested on 
`Kali Linux`

`Ubuntu 17.10 Server`


## Usage

```
python gpon_rce.py TARGET_URL COMMAND

```
e.g.
```
python gpon_rce.py http://192.168.1.15 'id'

```
