hellspy-synology
================

HellSpy.cz plugin for Synology DSM 3.2+ Download Station. Allows premium users to download files just by pasting their URLs.


Binary version that you can load directly into Synology's Download Station:
https://dl.dropboxusercontent.com/u/25376807/hellspy.host


How to build:
-------------

Pack "hellspy.php" and "INFO" files using tar-gzip format.

On Windows you can use for example Total Commander to do that, on Linux use tar utility.


How it work's
-------------

Plugin is using HellSpy API originally used for HellSpy Download Manager, no web-pages are being parsed and everything is loaded using API calls.