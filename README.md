# WP2Static

A fork of a WordPress plugin for static site generation and deployment.

---
## Installation

 - Requirements: composer, zip
 - git clone https://github.com/swtrse/wp2static.git
 - cd wp2static
 - composer install
 - Optional: composer test
 - composer build wp2static
 - cd ~/Downloads
 - Take the zip file and upload the plugin in the wordpress admin panel 
 

## Differences to original version

 - /robots.txt only get added to the detection list if the option is choosen
 - /favicon.ico only get added to the detection list if the option is choosen
 - /sitemap.xml only get added to the detection list if the option is choosen
 - Archive Pages based on date only get added to the detection list if the option is choosen
 - Archive Pages based on author only getadded to the dectection list if the option is choosen
 - Contact forms of "Contact Form 7" that only are shown in the admin backend no longer get added to the detection list
 - SuperCache entries no longer get added to the detection list
 - verndor cache only get addet to the dectection list if option is choosen (This does address the case where cached files from SuperCache got added to the URL list even if cache is handled via ngix or other ways, however since cached files should only be used implicit I see no point in keeping this option, however for compatibility I added the option for the user to choose maybe there are cases where this is usefull)

 ## Configuration Nodes

 After playing around quite a bit with this plugin I did come to the conclusion that in most cases, especially if you do not use wordpress for blogging, every detection option can be deactivated.
 The only exception is either robots.txt if it contains the sitemap url or the sitemap option. If the sidemap is complete and correct every page visible should be crawled correctly and no other detection method is necesary.

## Version Numbering

Version numbering is a bit different for this plugin. The Version number will be the wp2static version number this fork is based on and compatible to. Based on my time at hand I will try to keep up with changes.