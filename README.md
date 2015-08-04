freshBuntu
==========
What to do when Jon wants a fresh install of Ubuntu. 


Bash Aliases
===========
`vim ~/.bash_aliases`

```
alias get='sudo apt-get install'

gs () {
  cd ~/Projects/growsumo
  source ~/.bashrc
  workon gs
  gunicorn -b 0.0.0.0:3000 --worker-class socketio.sgunicorn.GeventSocketIOWorker run:app
#  python run.py go
}

go (){
  gunicorn -b 0.0.0.0:3000 --worker-class socketio.sgunicorn.GeventSocketIOWorker run:app
}


gsfolder () {
  cd ~/Projects/growsumo
}


gstart() {
  gnome-terminal --working-directory=/home/jonathan/Projects/growsumo --geometry=110x20+5093+32 &
  gnome-terminal --working-directory=/home/jonathan/Projects/growsumo --geometry=110x20+5093+382 &
  gnome-terminal --working-directory=/home/jonathan/Projects/growsumo --geometry=110x20+5093+760 &
}
```



Remove Sudo Password Prompt
==========
`sudo vim /etc/sudoers`

Change the line (25) `%sudo ALL=(ALL) ALL` to `%sudo ALL=(ALL) NOPASSWD: ALL`


Chrome
==========
https://www.google.com/intl/en/chrome/browser/ 


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



BashRC Prompt
===========
http://bashrcgenerator.com/

`export PS1="\[\e[00;31m\]\A\[\e[0m\]\[\e[00;37m\] @ \[\e[0m\]\[\e[00;33m\]\w\[\e[0m\]\[\e[00;37m\]: \[\e[0m\]"`


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


Virtualenv and wrapper
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


Inkscape
============
https://inkscape.org/en/download/linux/


Disable Ubuntu Guest Session
===================
`gksu gedit /etc/lightdm/lightdm.conf`

Append the following `allow-guest=false`


Ruby & Compass
============
`sudo apt-get install ruby`
`sudo apt-get install ruby-dev`
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


Atom.io
=====================
https://atom.io/

Theme:

Pacakages:

Macros:

