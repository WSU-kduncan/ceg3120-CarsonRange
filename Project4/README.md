# Part 2
## 1. 
* At the top of `/etc/hosts` there is ip address and then the hostname is leads to, this makes it so your system has a hostname that is in no way connected to the hostname of the ip you are connecting to, 
* while in the `.ssh/config` file you need to direct the key to it, and set hostname and users


## 2. 
* if you did everything I described in step 1 the commands below should work 
```
ssh Web-Server-1

ssh Web-Server-2
```

## 3.
* google the config file and change it as you need for your proxy, and verify it with `haproxy -f /etc/haproxy/haproxy.cfg -c` and once its correct do `sudo systemctl restart haproxy` to have the proxy up and running

* The only file I modified was `haproxy.cfg` at `/etc/haproxy/haproxy.cfg`

* There were default config file, however I deleted all of them and replaced them with my own

* `sudo systemctl restart haproxy`

* https://www.haproxy.com/blog/the-four-essential-sections-of-an-haproxy-configuration/ https://www.haproxy.com/blog/the-four-essential-sections-of-an-haproxy-configuration/

## 4.
* i moved the 2 .html files to the default html diretory and renamed them so they would work

* none of the webserver settings are changed

* in `/var/www/html` im guessing this is just how it works

* `sudo systemctl restart apache2`

## 5
![Server 1](server1.PNG)

![Server 2](server2.PNG)

## 6
* http://54.209.198.55/


(may not be running)