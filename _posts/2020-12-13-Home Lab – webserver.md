A project this year was to build a public-facing webserver that hosts hobbies. It promotes responsible ways to use our time, during this COVID-19 isolation, and was an opportunity for me to learn new skills.

This included learning the terminal for headless Ubuntu 18.04, Docker Compose, Nginx, LetsEncrypt, Fail2ban, Rclone, custom logging and creating actions based on those logs. My favorite part was hardening the server and I'll list those methods here:

* Source-restricted SSH
* Automatic updates on each layer, with reboot windows available when needed. Ubuntu is automatically updating Docker engine, but Docker Compose (and containers) needed to be scripted. The download link for Compose does need to be manually changed in the script every so often, but that is quick…would be nice if Docker had a static link for the newest version.
* Fail2ban: added custom definitions to deny traffic after x unsuccessful login attempts
* LetsEncrypt: using a limited-access Cloudflare API key (rather than storing login credentials) to maintain an SSL Certificate
* Rclone: leveraging a limited-access Google Drive API key for content

Over the past few months, it has been able to maintain 99.9% uptime and I haven’t had to do any manual maintenance or troubleshooting.

At some point, I’ll probably implement log rotation. This was super fun - a big part of that is sharing a personal project with family and friends. At some point in the future, I’d like to build something used by a broad community. Being able to contribute is a great feeling.
