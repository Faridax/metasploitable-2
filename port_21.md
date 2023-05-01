###  description 
> Attacking on port 21 

using ifconfig command to get my IP address!
>10.0.2.15


![1](https://user-images.githubusercontent.com/130427754/235381690-9383ad82-e20e-438b-8cb1-ce3a479ae39b.png)

### using nmap to scan the netwrok and using -sV flag which detect the version of the network services
 we get that metasploitable2 IP is `10.0.2.5` and it's running on linux OS! 
 
![2](https://user-images.githubusercontent.com/130427754/235381692-841d4a8a-9270-46a3-a681-341132df0c09.png)

focusing on `ftp` service on `port 21` and using NSE script by using flag `-sC`

found that Anonymous ftp login allowed! 

![3](https://user-images.githubusercontent.com/130427754/235381703-761972ae-6995-435f-8240-3be2ccf401a5.png)

trying to login by Anonymous

`LOGIN SUCCESSFUL!`

![4](https://user-images.githubusercontent.com/130427754/235381705-d0278c47-a3dc-4d81-bfbd-999cea48354e.png)

### using `hydra` fast login cracker tool with wordlists for different usernames and passwords 

found another login credentials

![5](https://user-images.githubusercontent.com/130427754/235381727-1de8d15e-decb-4793-995b-c03ca5f86efc.png)

trying to login with `user` as username and password 

![6](https://user-images.githubusercontent.com/130427754/235381733-254bb245-c024-4643-914f-b893065e225e.png)

`LOGIN SUCCESSFUL!`


