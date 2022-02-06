#Get started with raspberry pi

Download Raspberry OS from this link
```
https://www.raspberrypi.org/downloads/raspberry-pi-os/
```

Downmoad balena etcher to transfer the zip file onto the sd card of your raspberry
```
https://www.balena.io/etcher/
```
on balena etcher upload the OS zip onto the root sd card

once it's done put the sd card back in the raspberry 

## Set up wifi 
put your sd card in your computer and create a file named wpa_supplicant.conf
and write the following code
```
country=//country 2 letter code
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1

network={
  ssid=//wifi_name
  psk=//wifipassword
}
```
create a file named ssh without any code and put the sd card back in your rapberry
 

##set up ssh
Default name : pi
Default password : raspberry
Default hostname : raspberrypi

in your terminal write
```
ssh pi@raspberrypi.local
````
enter the default password and the connection is established via ssh

```
sudo apt-get update;
sudo apt-get upgrade;
````
to make sure everything is up to date


 
