# kkh-autologin
Automatically login into the Mikrotik RouterOS Authentication and access the panel along with some hacks using your favorite CLI

## KKH AutoLogin
  KKH autologin is an open source CLI tool to automatically\nlogin to the network RouterOS authentication panel.
  This script automatically tries out all the passwords\nspecified into the passfile (which can be edited) until login succeeds.
    
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

