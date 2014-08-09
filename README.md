freshBuntu
==========

What to do when you have a fresh install of Ubuntu. 


Bash Aliases
===========
`vim ~/.bash_aliases`

`alias get='sudo apt-get install'`

`syd () {`
  `cd ~/Dropbox/yunite-development/yunite`
  `source ~/.bashrc`
  `workon yunite`
  `python manage.py runserver`
`}`

`syd2 () {`
  `cd ~/Dropbox/yunite-development/yunite2`
  `source ~/.bashrc`
  `workon yunite2`
  `python run.py dev`
`}`

`yd () {`
  `cd ~/Dropbox/yunite-development/yunite`
`}`

`yd2 () {`
  `cd ~/Dropbox/yunite-development/yunite2`
`}`

`pullonben () {`
  `git pull origin ben-dev`
`}`

`pullonneil() {`
  `git pull origin neil-dev`
`}`


Remove Sudo Password Prompt
==========
`sudo vim /etc/sudoers`

Change the line (25) `%sudo ALL=(ALL) ALL` to `%sudo ALL=(ALL) NOPASSWD: ALL`


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


Git  - Reinstall
==========
`rm ~/.gitconfig`

`sudo apt-get purge git`

`sudo apt-get autoremove`

Git - Install
==========
`get git`

`git config --global user.name "Your Name"`

`git config --global user.email you@example.com`

Git - Setting up a remote 
==========
`git remote add origin git@github.com:user/repo.git`

Verify:
`git remote -v`

Git - Setting up a project
==========
http://gitref.org/creating/#clone

Git - Resetting to the master branch
==========
`git fetch origin`

`git reset --hard origin/master`


DropBox
==========
https://www.dropbox.com/download?dl=packages/ubuntu/dropbox_1.6.0_amd64.deb


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


Google Voice
==============
https://www.google.com/tools/dlpage/hangoutplugin/thankyou.html?platform=linux_ubuntu_x86_64


Gimp
===========
`sudo apt-get install gimp`


VLC
============
`sudo apt-get install vlc`


Disable Ubuntu Guest Session
===================
`gksu gedit /etc/lightdm/lightdm.conf`

Append the following `allow-guest=false`


Compass
============
`sudo gem install compass`


Node/NPM
=====================
`sudo add-apt-repository ppa:chris-lea/node.js`
`sudo apt-get update`
`sudo apt-get install nodejs`

Confirm

`node --version`
`npm -v`


Grunt
=====================
`npm install -g grunt-cli`


Sublime Text Editor
=====================
Make sure you're the owner of the directory via the next 2 commands:
`sudo chown -R {youruser}:{youruser}  "/home/{youruser}/.config/sublime-text-2"`
`sudo sublime`

Install the Package Control Manager via the following link: 
https://sublime.wbond.net/installation#st3

Install Brogrammer Theme
https://github.com/kenwheeler/brogrammer-theme

Install the following packages:
- AngularJS
- AutoFileName
- ColorPicker
- CSS3
- Emmet
- EmmetCssSnippets
- ExpandSelectiontoQuotes
- Djaniero
- GitGutter
- JSHintGutter
- LiveStyle
- Open project path by shortcut
- PackageControl
- Placeholders
- Python3
- PyV8
- SCSS
- SCSS Snippets
- SearchAnywhere
- SublimeLinter
- SyntaxHighlightingforSASS
