# All in One Recon Tool

`An easy-to-use python tool to perform dns recon, subdomain enumeration and much more`

The purpouse of this tool is helping bug hunters and pentesters during reconnaissance

If you want to know more about the tool you can read my own [post](https://d3ext.github.io/aort) in my blog (written in spanish) 

## Installation:
It can be used in any system with python3

You can easily install AORT using pip:

```sh
pip3 install aort
```

If you want to install it from source:
```sh
git clone https://github.com/trhacknon/AORT
cd AORT
pip3 install -r requirements.txt
```

> One-liner
```sh
git clone https://github.com/trhacknon/AORT && cd AORT && pip3 install -r requirements.txt && python3 AORT.py
```

## Usage:

- Common usages

> If installed with pip3:
```sh
aort
```

> To see the help panel and other parameters
```sh
python3 AORT.py -h
```

> Main usage of the tool to dump the valid domains
```sh
python3 AORT.py -d example.com
```

> Perform all the recon
```sh
python3 AORT.py -d domain.com --all
```
## Features:

:ballot_box_with_check: Enumerate subdomains using passive techniques (like **subfinder**)

:ballot_box_with_check: A lot of extra queries to enumerate the DNS

:ballot_box_with_check: Domain Zone transfer attack

:ballot_box_with_check: WAF type detection

:ballot_box_with_check: Common enumeration (CMSs, reverse proxies, jquery...)

:ballot_box_with_check: Whois target domain

:ballot_box_with_check: Subdomain Takeover checker

:ballot_box_with_check: Scan common ports

:ballot_box_with_check: Check active subdomains (like **httprobe**)

:ballot_box_with_check: Wayback machine support to enumerate endpoints (like **waybackurls**)

:ballot_box_with_check: Email harvesting

## Todo:

- Compare results with other tools such as **subfinder**, **gau**, **httprobe**...

## Demo:

> Simple query to find valid subdomains
<img src="https://raw.githubusercontent.com/trhacknon/AORT/main/demo.png">

## Third part

The tool uses different services to get subdomains in different ways

The WAF detector was modified and addapted from [CRLFSuite](https://github.com/Nefcore/CRLFsuite) concept

All DNS queries are scripted in python at 100%

Email harvesting using Hunter.io API with personal token (free signup)

## Extra

**If you consider this project has been useful, I would really appreciate supporting me by giving this repo a star or buying me a coffee.**

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/d3ext)

Copyright © 2022, *D3Ext*
