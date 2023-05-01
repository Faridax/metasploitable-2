###  description 
> Attacking on port 25

using nmap to scan port 25 and using -sC flag to run NSE script on it

![smtp1](https://user-images.githubusercontent.com/130427754/235384025-f2496b6e-d23d-4f4b-8243-275a5a389bb9.png)

in another terminal ==> using msfconsole for interacting with the Metasploit Framework
then `search smtp`

![smtp2](https://user-images.githubusercontent.com/130427754/235384030-7759964a-0bc9-4a57-a025-3e156e8807fd.png)

search for smtp enumeration `smtp_enum` and then `use 0`

![smtp3](https://user-images.githubusercontent.com/130427754/235384035-8f38e22e-c94c-4940-b969-ece9fdf46539.png)
 found `USER_FILE` then copy the path of the file to read the file's input using `cat` command!

![smtp4](https://user-images.githubusercontent.com/130427754/235384041-82d724e6-11b4-424d-8aca-7c593bcb56d3.png)

found many usernames for different users!

![smtp5](https://user-images.githubusercontent.com/130427754/235384047-edc7d5e9-0e80-4e03-b0ec-a8face47382e.png)

trying `smtp-user-enum` command with a wordlist for usernames to find out if a certain users exists 

9 users are found!

![smtp6](https://user-images.githubusercontent.com/130427754/235384050-1972d719-586e-4276-8d97-d8aa6be760ba.png)

typing `run` in ms console , we found many usernames!

![smtp7](https://user-images.githubusercontent.com/130427754/235384053-d40bcacc-aa02-404b-8d17-f85dd1a6537b.png)

