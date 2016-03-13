# kkh-autologin
Automatically login into the Mikrotik RouterOS Authentication and access the panel along with some hacks using your favorite CLI

### About
  KKH autologin is an open source CLI tool to automatically login to the network RouterOS authentication panel.
  This script automatically tries out all the passwords specified into the passfile (which can be edited) until login succeeds.
### Why I made this? And why do I use it?
  * Whenever I connect to my hostel wifi network, I am asked to log in to the authentication portal. I was sick of logging in everytime I connect. 
  * There is only one session allowed per username in the portal and due to obvious unchangable username-password combination, if a person logged in using your credentials, you cannot login using the same username until that person logs out. So, you need to try out any other person's credentials to see if it gets you logged in.
  * Manually typing in and trying out 5-10 username-password combinations depending upon luck is very tedious. So, I wrote a script that does that automatically and when my password file is completed checking all credentials or login is successful, it exits.
  * So, I just type in `$ kkh hack` into my terminal and within a few seconds, I am logged in automatically.
  * You can customize it according to your need and ip addresses. This saves me around 20-30 minutes everyday :-)

## Installation
  Clone this repo, move kkh and passfile to any location from PATH (preferably /usr/local/bin) and give it execute permissions.
    $ git clone git@github.com:lokeshthegenius/kkh-autologin.git
    $ cd kkh-autologin
    $ mv {kkh,passfile} /usr/local/bin/
    $ chmod +rx kkh passfile
    $ vi passfile            # add your usernames and passwords
    
    
## Features  
  1. Check status :  kkh status
  2. Log in        :  kkh login [username [password]]
  3. Log out       :  kkh logout
  4. Autologin all :  kkh hack [file]
  
## Documentation    
####  1. Checking status
    $ kkh status
####  2. Login
    a) $ kkh login
    b) $ kkh login john
    c) $ kkh login john johnpassword
####  3. Logout
    $ kkh logout
####  4. Autologin all [Try every username password in passfile until login is Successful]
    a) $ kkh hack";
    b) $ kkh hack passfile";
    
## Developer
  Made with love by Lokesh Devnani


