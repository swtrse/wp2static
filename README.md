# WP2Static

A fork of a WordPress plugin for static site generation and deployment.

---
## Installation options

 - from this source code `git clone https://github.com/swtrse/wp2static.git` (run `composer install` afterwards)

## Differences to original version

 - /robots.txt only get added to the detection list if the option is choosen
 - /favicon.ico only get added to the detection list if the option is choosen
 - /sitemap.xml only get added to the detection list if the option is choosen
 - Archive Pages based on date only get added to the detection list if the option is choosen
 - Archive Pages based on author only getadded to the dectection list if the option is choosen
 - Contact forms of "Contact Form 7" that only are shown in the admin backend no longer get added to the detection list
