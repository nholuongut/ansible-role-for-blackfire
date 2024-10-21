# Ansible Role: Blackfire

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

Installs [Blackfire](https://blackfire.io/) on RHEL/CentOS or Debian/Ubuntu.

## Requirements

After installation, you need to complete Blackfire setup manually before profiling:

  1. Register the Blackfire agent: `sudo blackfire-agent -register`
  2. Configure Blackfire: `blackfire config`

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    blackfire_packages:
      - blackfire-agent
      - blackfire-php

The Blackfire packages this role will install on the server. Note that `blackfire-php` may not work well with XHProf and/or XDebug.

    blackfire_gpg_key_url: https://packages.blackfire.io/gpg.key
    blackfire_repo_url: http://packages.blackfire.io/fedora/blackfire.repo

Variables used for Blackfire package setup and installation.

## Dependencies

Requires the `nholuong.php` role.

## Example Playbook

    - hosts: webserver
      roles:
        - nholuong.php
        - nholuong.blackfire

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟