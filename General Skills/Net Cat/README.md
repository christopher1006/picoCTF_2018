# Net Cat - General Skills
## Points: 75

## Question 
  > Using netcat (nc) will be a necessity throughout your adventure. Can you connect to 2018shell.picoctf.com at port 49387 to get the flag?
## Hint
  > nc tutorial (https://linux.die.net/man/1/nc)
## Solution
  > Install netcat
  > Run `nc -p SOURCE_PORTNUMBER* 2018shell.picoctf.com 49387`
  > Upon succesful TCP connection, the flag is returned.
  > * Note SOURCE_PORTNUMBER must be an integer matching a usable source port
### Flag
`picoCTF{NEtcat_iS_a_NEcESSiTy_8b6a1fbc}`
