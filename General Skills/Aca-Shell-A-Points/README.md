# Aca-Shell-A-Points

## Points: 150

## Question 
  > It's never a bad idea to brush up on those linux skills or even learn some new ones before you set off on this adventure! Connect with `nc 2018shell.picoctf.com 42334`.

## Hint
  > Linux for Beginners (https://maker.pro/linux/tutorial/basic-linux-commands-for-beginners)
## Solution
 Connect to the server with `nc 2018shell.picoctf.com 42334`
 
 Follow the prompt and go to the secret folder.
 `cd secret`
 `ls`
 Remove only the files labeled intel.
 `rm intel*`
 Follow the prompt by parroting the echo command.
 `echo Drop it in!`
 Move to executables folder
 `cd ..`
 `cd executables`
 `ls`
 Execute dontLookHere
 `./dontLookHere`
 Identify the active username.
 `whoami`
 Back out to home directory and copy the tmp file over to the passwords folder.
 `cd ..`
 `cp /tmp/TopSecret passwords`
 `cd passwords`
 Print the TopSecret file.
 `cat TopSecret`
 Flag is to be found at the very end of the string output.
### Flag
`picoCTF{CrUsHeD_It_d6f202f1}`
