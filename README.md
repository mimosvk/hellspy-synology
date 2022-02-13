hellspy-synology
================

*HellSpy.cz* | *HellSpy.sk* | *HellSpy.com* host config for Download Station on Synology NAS.

Allows premium users to download files just by pasting their URLs.

**Tested only with DSM 7.0 on Synology DS118.**

Synology Download Station needs only file called "hellspy.host" to work.
* If you are using **hellspy.cz**  please download only `./hellspy.cz/hellspy.host` file from this repository .
* If you are using **hellspy.com** please download only `./hellspy.com/hellspy.host` file from this repository .
* If you are using **hellspy.sk**  please download only `./hellspy.sk/hellspy.host` file from this repository .

How it work's
-------------

You need to:
1. open your Synology DSM,
2. go to Download Station,
3. click on "wheel" icon in left bottom corner,
4. browse to "File Hosting",
5. click on "Add" button,
6. load your "hellspy.host" file from disk and click on "add",
7. find "hellspy" in "File Hosting" list and fill your credentials to HellSpy,
8. copy URL from HellSpy site you want to download,
9. paste yhis URL to Download Station in your Synology NAS.

Plugin is using HellSpy API originally used for HellSpy Download Manager, no web-pages are being parsed and everything is loaded using HellSpy API calls.

How to build:
-------------

Pack "hellspy.php" and "INFO" files using tar+gzip format but with `.host` extension not `.tar.gz` . On Linux for example you may run:
```bash
#!/bin/bash
chmod -v 0755 INFO
chmod -v 0755 hellspy.php
tar -czvf ./hellspy.host ./INFO ./hellspy.php
```

-------------------------------------------------------------------------------

Forked from [AfBu/hellspy-synology](https://github.com/AfBu/hellspy-synology) and fixed for SK | CZ | COM versions of HellSpy site.
