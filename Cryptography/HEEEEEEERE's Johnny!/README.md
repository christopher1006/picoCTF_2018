# HEEEEEEERE'S Johnny! 

## Points: 100

## Question 
  > Okay, so we found some important looking files on a linux computer. Maybe they can be used to get a password to the process. Connect with `nc 2018shell.picoctf.com 40157`. Files can be found here: `passwd` `shadow`.
## Hint
  > If at first you don't succeed, try, try again. And again. And again.
  
  > If you're not careful these kind of problems can really "rockyou".
## Solution
  > Download John The Ripper (https://www.openwall.com/john/) or install it from official package managers.
  
  > First, combine the shaddow and password files togther `unshadow passwd shadow > combinedPW`
  
  > Using the `rockyou.txt` wordlist as an argument, attempt to crack the new password file `john --wordlist=rockyou.txt combinedPW`.
  
  > Either `cat` the `combinedPW` file or `john -show combinedPW` which results in `root:password1:0:0:root:/root:/bin/bash`
  
  > Connect to server, using `root` and `password1` in their respective fields to retrieve the flag.
  
  Referenced https://www.cyberciti.biz/faq/unix-linux-password-cracking-john-the-ripper/ for using John The Ripper.
### Flag
`picoCTF{J0hn_1$_R1pp3d_1b25af80}`
