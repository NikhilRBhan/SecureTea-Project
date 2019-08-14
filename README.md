<img align="left" width="120" height="120" src="img/logo/secure-tea-white.png">

# [OWASP SecureTea][SecureTea-OWASP]

[![Build Status][Travis-badge]][Travis]
[![Codacy Badge][Codacy-badge]][Codacy]
[![PyPI][PyPi-badge]][PyPi]
[![GitHub][License-badge]][License]
[![Telegram][Telegram-badge]][Telegram]
[![Version][Version-badge]][Version]
[![Tag][Tag-badge]][Tag]
[![GitHub issues][Issues-badge]][Issues]
[![GitHub pull requests][PR-badge]][PRs]
[![GSOC 2019][GSOC-2019-badge]][GSOC-OWASP]
[![Follow Us](https://img.shields.io/twitter/url/https/secureteatool.svg?label=SecureTea%20Project&style=social)](https://twitter.com/secureteatool)
[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors)

**The OWASP SecureTea Project** provides a one-stop security solution for various devices (personal computers / servers / IoT devices).<br>
The **core** feature includes the following:
- [x] Intrusion Detection System
- [x] Firewall
- [x] AntiVirus
- [x] Server Log Monitor
- [x] System Log Monitor
- [x] Local Web Deface Detection & Prevention System
- [x] Auto Web Server Patcher
- [x] IoT Anonymity checker
- [x] Auto report generation using OSINT
- [x] Notifying suspicious activities using various mediums (Twitter, Telegram, Slack, Gmail, SMS, AWS & more)
- [x] Interactive GUI for ease of setting up

![Setup Intro][Setup-help-animation]

## Table Of Contents
-   [Pre-requisites](#pre-requisites)
-   [Installation Procedure](#installation-procedure)
-   [Quick Start](#quick-start)
-   [Suggestions and Contribution](#suggestions-and-contributing)
-   [Code Of Conduct](/CODE_OF_CONDUCT.md)
-   [User guide](/doc/en-US/user_guide.md)
-   [Developer guide](/doc/en-US/dev_guide.md)
-   [Translation-Japanese](/doc/ja-JP/README.md)
-   [Translation-Hindi](/doc/hi-IN/README.md)
-   [License](#license)

## Pre-requisites
#### Supported Platforms
OWASP SecureTea Tool project runs on Linux operating systems.

#### Hardware
-  Linux OS / Raspberry Pi - have `sudo` access on the terminal/console
-  Mouse / Wireless Mouse / Touchpad congenital laptop

#### Software
-  Python 2.x or 3.x
-  Angular
-  Twitter account (optional)
-  Telegram account (optional)
-  Slack account (optional)
-  Twilio SMS account (optional)
-  Amazon Web Services account (optional)
-  Libnetfilter
-  Yara
-  Clam AV

#### Installing pre-requisites
Python:<br>
https://www.python.org/

Angular:<br>
https://angular.io/

Libnetfilter:<br>
https://www.netfilter.org/projects/libnetfilter_queue/
```command
sudo apt-get update
sudo apt-get install build-essential python-dev libnetfilter-queue-dev
```

Yara:<br>
https://yara.readthedocs.io/en/v3.7.0/gettingstarted.html
1. Download the latest Yara release at: https://github.com/VirusTotal/yara/releases
2. Execute the following instructions in the order:
```command
tar -zxf yara-3.10.0.tar.gz
cd yara-3.10.0
./bootstrap.sh
sudo apt-get install automake libtool make gcc
sudo apt-get install flex bison
./configure
make
sudo make install
make check
```

Clam AV:<br>
https://www.clamav.net/
1. Execute the following instructions in the order:
```command
sudo apt-get install clamav
sudo freshclam
```

## Installation Procedure

You can install SecureTea from PyPi package manager using the following command:

`pip install securetea`

Please make sure all dependencies are installed if this fails.<br>
For more detailed information, refer to the [installation guide](https://github.com/OWASP/SecureTea-Project/blob/master/doc/en-US/user_guide.md#installation)

## Quick Start

1. Start SecureTea in [**server mode**](https://github.com/OWASP/SecureTea-Project/blob/master/doc/en-US/user_guide.md#starting-up-in-server-mode):<br>
`sudo SecureTea.py --server-mode`

2. Start SecureTea in [**system mode**](https://github.com/OWASP/SecureTea-Project/blob/master/doc/en-US/user_guide.md#starting-up-in-system-mode):<br>
`sudo SecureTea.py --system-mode
`
3. Start SecureTea in [**IoT mode**](https://github.com/OWASP/SecureTea-Project/blob/master/doc/en-US/user_guide.md#starting-up-in-iot-mode):<br>
`sudo SecureTea.py --iot-mode`

### User Guide

Read detailed [user guide](/doc/en-US/user_guide.md).

### Developer Guide

Read detailed [developer guide](/doc/en-US/dev_guide.md).

## Suggestions and Contributing

See more at [Contributing Guide](/CONTRIBUTING.md).

## Project Leaders

-   [Ade Yoseman][Ade]
-   [Rejah Rehim][Rejah]


| **Chat Group** | **Google Summer of Code** | **YouTube** |
| -------------- | ------------------------- |---------------------|
| [<img src="/img/telegram.png" width="50" title="Telegram">][Telegram]  | [<img src="/img/GSoC-logo.jpg" width="100"></img>][GSOC-OWASP]  | [<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b8/YouTube_Logo_2017.svg/1024px-YouTube_Logo_2017.svg.png" width="90" title="YouTube">][YouTube] | 

[YouTube]: https://www.youtube.com/channel/UCGdl9tpc1qZYcM3WRRFRPPA
[OWASP-logo]: https://github.com/OWASP/Amass/blob/master/images/owasp_logo.png
[SecureTea-OWASP]: https://www.owasp.org/index.php/OWASP_SecureTea_Project
[GSOC-OWASP]: https://summerofcode.withgoogle.com/organizations/6362925392986112/
[Telegram]: https://t.me/joinchat/Az5yZxQg7Djs-UZWKKCRVQ
[Telegram-badge]: https://img.shields.io/badge/chat%20on-telegram-blue.svg
[Codacy]: https://app.codacy.com/app/rejahrehim/SecureTea-Project?utm_source=github.com&utm_medium=referral&utm_content=OWASP/SecureTea-Project&utm_campaign=Badge_Grade_Settings
[Codacy-badge]: https://api.codacy.com/project/badge/Grade/7e1de11511084c06bbe25ed4d629e7fd
[Travis-badge]: https://travis-ci.com/OWASP/SecureTea-Project.svg?branch=master
[Travis]: https://travis-ci.com/OWASP/SecureTea-Project
[PyPi]: https://pypi.org/project/securetea/
[PyPi-badge]: https://img.shields.io/pypi/v/securetea.svg
[GSOC-2019-badge]: https://img.shields.io/static/v1.svg?label=GSOC&message=Google%20Summer%20of%20Code%202019&color=blue&logo=%20data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAAXNSR0IArs4c6QAABLFJREFUSA2tVV1sVFUQ/s45d7ulpT+63VSkQC1IIsHyAugDAWLwQSEQI/EnaGL0QWOQ6AMo+uAzJooJJJiIiQ8qkWDURIxGIlLUqEQTKz9REEpbMFhKt7ss7e49P35zb9jaqKEkTnL33jNn5ps538ycBa5D7MH8etuTX38dLlM3jQ+2rXRf1Q/LI99T9VRTMYy/rF+hUflAIeTEPkANe2Tvz9w1fuha/pMChE/RbDNRd83JWnigwzTO2Gma5+ec6eCWgnEDcMXfhl35j43cH4yiqOYSxbZX3YviVcXEDjVWR4tMRvUEegUXQzfNRtT1PJBbw7WFjocTv5DJwZgoZy7t3+N/34YwdhbKZKA0MO6i5UQ6/K8BYBC8gNsYKr8a6rZdCJePwx97EmH0e+rTxFTUDNW8FHrOs9CLD8OdeBp+6BOoKAPBuAou70knSDaYucrfA73wXbhTW+EHdqX2ypCdlNHgigjDn8Pz0R1PwSx8B+7oBuDi/n9ATgoQW+vqp8+EWrCb4C/B9xPciMnfSuVjLhlMM1sm6/vfSNZmwZvwR5YilAZdmlH6S9YmxFjMVl2bEcon08wTcO4LqEhwMHNfhm65E+BJE2GB/SCpLP8K3bUFgpFupL+1AGNfTF8ZtbbtQNt9zOo17iaV5ltDz3iErzpyTO7bH6KOBZ/xYHoSBmXl4M++ymZYh6g1v0OwaJRIEiBwcOrMlX26cV4+eAU/+l2yqTJtiLr3Qd1EMDsONNzKzMvwpaPUbYC5fS9AG5FQZBMwJ8EQLMEUvbaH2tZ6lD4kbM7pmwl0CagOQzXOh1ncg1D9E66XWTNT1byELXmaNmW4Xx6m3RAi2ohtqNLPjsCZmTyzzwmmPdS+VhvYQmBp0gaRDmNBZSG829GUFtPAAFS33AEUf0i/RUfK6E7bqiRLkWYQQ/kOJYNKQasVhR7nMmt8QJ/xA3S6EUJNGDsD++MqHvsKqXiPgaZBNTDT4hGeO6JuT0KX/elu2vZB1eUTX8EQLEtMwU5qkF1V7rUe6/zlU6eV5hzcsDxJBH4M7tjjaQEbyT8n2JdPEKiOjbAd7vgTDDKWJt26jJPMq6V08rRgCaaco9ZF2VXoDcXCJlzYwwndzP5nnwtVnH8/9JkcGf7cbiAm16TED3Go5G4QG86E7qQPfePiyCbBEnCRWgBZhAxG/JnXSRHvms4XmJ0VbRIsuTL6XuFaCE5Bkz25o27ZklDkz2yHJwYNajJpksmtDvEQaXkUZtFHiZHr28ZALKJmLuQ+AZV+5KWlDGdj7laY2c/B/byOpxvioSIaSmKpTA5AnSY1vvANPB30greg82vg+ncgFA4nbZm4ZdugWpcT+BnWowW+l+CFr9PLzkonTsjkAKSbHTDuFfkf+ZZ3yzLoWRvrzLwXdVDSkqW0EU0T3yX48+97P7CzGqoXmTl9iB2IMQGfElpbh72YhvZsR6VCVZYPP0wFM9X0prdNU+ccpziIpN+E8/zD6TsbLpcec1mcE2Mxl5/BC5XBWQ+ArZWKVOyaUjlQ1x3p+GOtQqcY+6D6rM+wFau1bvkvkCkFEOfKgcbuyMTsTTLlMquv9rms/zepHmheIs/1AP4F9DYB6+AcwCcAAAAASUVORK5CYII=
[License]:  /LICENSE
[License-badge]: https://img.shields.io/github/license/mashape/apistatus.svg
[Version]: https://github.com/OWASP/SecureTea-Project/releases
[Version-badge]: https://img.shields.io/github/release/OWASP/SecureTea-Project.svg
[Tag]: https://github.com/OWASP/SecureTea-Project/tags
[Tag-badge]: https://img.shields.io/github/tag/OWASP/SecureTea-Project.svg?color=orange&label=version
[Issues]: https://github.com/OWASP/SecureTea-Project/issues
[Issues-badge]: https://img.shields.io/github/issues/OWASP/SecureTea-Project.svg
[PRs]: https://github.com/OWASP/SecureTea-Project/pulls
[PR-badge]: https://img.shields.io/github/issues-pr/OWASP/SecureTea-Project.svg
[Setup-help-animation]: /img/setup_all.gif
[Rejah]: https://rejahrehim.com
[Ade]: https://www.owasp.org/index.php/Ade_Yoseman_Putra

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table>
  <tr>
    <td align="center"><a href="https://abhisharma404.blogspot.com/"><img src="https://avatars0.githubusercontent.com/u/29058921?v=4" width="100px;" alt="Abhishek Sharma"/><br /><sub><b>Abhishek Sharma</b></sub></a><br /><a href="https://github.com/OWASP/SecureTea-Project/commits?author=abhisharma404" title="Code">💻</a> <a href="https://github.com/OWASP/SecureTea-Project/commits?author=abhisharma404" title="Documentation">📖</a></td>
    <td align="center"><a href="http://rejahrehim.com"><img src="https://avatars3.githubusercontent.com/u/4394746?v=4" width="100px;" alt="Rejah Rehim "/><br /><sub><b>Rejah Rehim </b></sub></a><br /><a href="https://github.com/OWASP/SecureTea-Project/commits?author=rejahrehim" title="Code">💻</a> <a href="https://github.com/OWASP/SecureTea-Project/commits?author=rejahrehim" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/adeyosemanputra"><img src="https://avatars1.githubusercontent.com/u/24958168?v=4" width="100px;" alt="adeyosemanputra"/><br /><sub><b>adeyosemanputra</b></sub></a><br /><a href="https://github.com/OWASP/SecureTea-Project/commits?author=adeyosemanputra" title="Code">💻</a> <a href="https://github.com/OWASP/SecureTea-Project/commits?author=adeyosemanputra" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/ananthus"><img src="https://avatars0.githubusercontent.com/u/30488894?v=4" width="100px;" alt="Ananthu S"/><br /><sub><b>Ananthu S</b></sub></a><br /><a href="https://github.com/OWASP/SecureTea-Project/commits?author=ananthus" title="Code">💻</a></td>
    <td align="center"><a href="http://sunn-e.github.io"><img src="https://avatars3.githubusercontent.com/u/30065288?v=4" width="100px;" alt="Sunny Dhoke"/><br /><sub><b>Sunny Dhoke</b></sub></a><br /><a href="https://github.com/OWASP/SecureTea-Project/issues?q=author%3Asunn-e" title="Bug reports">🐛</a> <a href="https://github.com/OWASP/SecureTea-Project/commits?author=sunn-e" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/kUSHAL0601"><img src="https://avatars3.githubusercontent.com/u/29600964?v=4" width="100px;" alt="MajAK"/><br /><sub><b>MajAK</b></sub></a><br /><a href="https://github.com/OWASP/SecureTea-Project/commits?author=kUSHAL0601" title="Code">💻</a></td>
    <td align="center"><a href="https://mishal23.github.io/"><img src="https://avatars3.githubusercontent.com/u/21958074?v=4" width="100px;" alt="Mishal Shah"/><br /><sub><b>Mishal Shah</b></sub></a><br /><a href="https://github.com/OWASP/SecureTea-Project/commits?author=mishal23" title="Code">💻</a></td>
  </tr>
</table>

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

## License
MIT License
