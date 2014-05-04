freshBuntu
==========

What to do when you have a fresh install of Ubuntu. 
Note that this will become a script in the near future.

Chrome
==========
Download it from the website silly: https://www.google.com/intl/en/chrome/browser/ 

AMD Processors: Choose 64 bit
Intel Processors: Choose 32 bit


GitHub Key Pair
==========
https://help.github.com/articles/generating-ssh-keys


SSH Client and Server
==========
`sudo apt-get install openssh-client`

`sudo apt-get install openssh-server`

Disable SSH password login
-----------
Change the line (51) `#PasswordAuthentication yes` to `PasswordAuthentication no`


Git
==========
`sudo apt-get install git`

`git config --global user.name "Your Name"`

`git config --global user.email you@example.com`


DropBox
==========
https://www.dropbox.com/download?dl=packages/ubuntu/dropbox_1.6.0_amd64.deb


Remove Sudo Password Prompt
==========
`sudo vim /etc/sudoers`

Change the line (25) `%sudo ALL=(ALL) ALL` to `%sudo ALL=(ALL) NOPASSWD: ALL`


BashRC Prompt
===========
http://bashrcgenerator.com/

`export PS1="\[\e[00;31m\]\A\[\e[0m\]\[\e[00;37m\] [\w] : @\[\e[0m\]"`


Linux Terminal
===========
Background Tab - ~50% Transparent background

Color Tab: 

![alt text](https://raw.githubusercontent.com//mstokes5/freshBuntu/master/images/color.png "Terminal Color Tab")

Terminal: 

![alt text](https://raw.githubusercontent.com//mstokes5/freshBuntu/master/images/term.png "Terminal Color Tab")

Gimp
===========
`sudo apt-get install gimp`


Bash Aliases
===========
`vim ~/.bash_aliases`

```alias get='sudo apt-get install'```
```alias back = 'cd...'```


VLC
============
`sudo apt-get install vlc`



Pip
============
`sudo apt-get install python-pip`


Virtualenv and Wrapper
============
http://roundhere.net/journal/virtualenv-ubuntu-12-10/


Postgres
============
https://www.digitalocean.com/community/articles/how-to-install-and-use-postgresql-on-ubuntu-12-04

And also: `sudo apt-get install libpq-dev`

Remember to change the pg_hba.conf:
`vim /etc/postgresql/{% version number, currently USING 9.1 %}/main/pg_hba.conf`
So that login settings are all of 'password' METHOD 


Python Dev
============
`sudo apt-get install python-dev`


Pgadmin3
============
`sudo apt-get install pgadmin3`


Private Internet Access
=============
https://www.privateinternetaccess.com/pages/client-support/#ubuntu_openvpn_installer


Google Voice
==============
https://www.google.com/tools/dlpage/hangoutplugin/thankyou.html?platform=linux_ubuntu_x86_64


Vimrc
==============
```sh
set nocompatible
set nocompatible
set number
set ruler
set backspace=indent,eol,start
set autoindent
set backup
set backupdir=~/.vim/backups
set history=100
set showcmd
set showmode
set incsearch
syntax on
set hlsearch
filetype plugin indent on
set wrap
set background=dark
set wrapscan
set mouse=a
set clipboard=unnamedplus

set tabstop=2
set shiftwidth=2
set expandtab

set nospell

let &printexpr="(v:cmdarg=='' ? ".
    \"system('lpr' . (&printdevice == '' ? '' : ' -P' . &printdevice)".
    \". ' ' . v:fname_in) . delete(v:fname_in) + v:shell_error".
    \" : system('mv '.v:fname_in.' '.v:cmdarg) + v:shell_error)"

```
also install 
vim-gui-common

Disable Ubuntu Guest Session
===================
`gksu gedit /etc/lightdm/lightdm.conf`

Append the following `allow-guest=false`


VirtualBox
====================
`get virtualbox`


Node/NPM
=====================
An absolute pain.


Grunt
=====================
Was painful because of above.


Sublime Text Editor
=====================
Make sure you're the owner of the directory via the next 2 commands:
- sudo chown -R {youruser}:{youruser}  "/home/{youruser}/.config/sublime-text-2"
- sudo sublime

Install the Package Control Manager via the following link: https://sublime.wbond.net/installation#st2

Install the following packages:
- Theme - Brogrammer
- SublimeLinter
- SFTP :: Add paid key to Package->SFTP->User - Settings
- Syntax Highlighting for Sass
- Color Picker
- CSS Snippets
- CSS Format
- CSS3_Syntax
- CSS Lint
- Djaniero
- Emmet
- Emmet CSS Snippets
- Jquery Snippets pack
- LiveStyle
- LiveReload
- Neat Sass Snippets
- Autoprefixer
- Placeholders
- Prefixr
- Python 3
- SCSS
- SCSS Snippets
- SASS Snippets
- Foundation 5 Snippets
- Search Wordpress Codes
- Wordpress
- Django-tools
- Search Anywhere
- Open Project Path by shortcut
