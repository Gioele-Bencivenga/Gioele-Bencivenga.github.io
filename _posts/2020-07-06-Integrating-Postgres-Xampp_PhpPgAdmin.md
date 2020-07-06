---
title: "Installing PostgreSQL in Xampp and Integrating PhpPgAdmin"
toc: true
categories:
  - Random Knowledge
tags:
  - Postgres
  - PhpPgAdmin
  - Xampp
  - Database
---

**Credits Time!**
This post is just a text version of [this video](https://www.youtube.com/watch?v=DFvBnsY15Bo).

I'm in no way affiliated with the author of the video.

I couldn't find a written explanation of how to do this when I was searching, so I thought about making a post.
{: .notice--primary}

## To Note

This guide assumes that we have already [installed xampp](https://www.apachefriends.org/download.html).

I haven't experimented with the paths and naming so I don't know if folder names and structure have to be set up like this in order for it to work.

## 1 - Install PostgreSQL

Download the installer [from here](https://www.postgresql.org/download/) and run it.

Set the installation path to `C:\xampp\pgsql\12` (the pgsql folder will need to be created, the folder named `12` needs to be created, I named it like that based on the current postgres version).

### 1.1 - Modify php Config

Navigate to `C:\xampp\php` and open `php.ini` with an editor like VSCode or Notepad++.

Uncomment (by removing the preceding `;`) the lines `extension=pgsql` and `extension=pdo_pgsql`.

Save the file.

## 2 - Install PhpPgAdmin

Download the master branch from the [repository](https://github.com/phppgadmin/phppgadmin) (Code > Download ZIP).

Extract the contents of the folder into any other folder.

Get the all of the contents (`CTRL + A`) of the extracted folder and move them into `C:\xampp\phpPgAdmin` (the folder `phpPgAdmin` will need to be created).

### 2.1 - Modify PhpPgAdmin Config

Go to `C:\xampp\phpPgAdmin\conf` and rename `config.inc.php-dist` to `config.inc.php`.

Open `config.inc.php` (again with Notepad++, VSCode or whatever).

Change the line `$conf['servers'][0]['host'] = '';` to `$conf['servers'][0]['host'] = 'localhost';`.

Change the lines `$conf['servers'][0]['pg_dump_path'] = '/usr/bin/pg_dump';` and `$conf['servers'][0]['pg_dumpall_path'] = '/usr/bin/pg_dumpall';` to `$conf['servers'][0]['pg_dump_path'] = 'C:\\xampp\\pgsql\\12\\bin\\pg_dump.exe';` and `$conf['servers'][0]['pg_dump_path'] = 'C:\\xampp\\pgsql\\12\\bin\\pg_dumpall.exe';`.

Change the line `$conf['extra_login_security'] = true;` to `$conf['extra_login_security'] = false;`.

Save the file.

## 3 - Modify Xampp Config

Search for the file `httpd-xampp.conf` and open it.

Right before the line `<IfModule alias_module>` insert this code snippet:

```Conf
Alias /phpPgAdmin "C:/xampp/phpPgAdmin"
<directory "C:/xampp/phpPgAdmin">
AllowOverride AuthConfig
Require all granted
</directory>
```

## 4 - Check if it Works

Check if everything went smoothly by going to `http://localhost/phpPgAdmin/`.

Click on the PostgreSQL server in the sidebar.

Login with the username `postgres` and the password you specified during PostgreSQL installation.
