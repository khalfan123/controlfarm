# Welcome to ControlFarmSystem

### Package Installation
> [https://www.openhab.org/download/](https://www.openhab.org/download/)
> 
1.  Add the repository key

```
wget -qO - 'https://bintray.com/user/downloadSubjectPublicKey?username=openhab' | sudo apt-key add -
```

3.  Add the HTTPS transport for APT

```
sudo apt-get install apt-transport-https
```

5.  Add the repository

```
echo 'deb https://dl.bintray.com/openhab/apt-repo2 stable main' | sudo tee /etc/apt/sources.list.d/openhab2.list
```

7.  Update the package lists and install the openHAB distribution package

```
sudo apt-get update && sudo apt-get install openhab2
```

9.  **(Optional)**  Install the add-ons for offline use
🛈  You don't need the add-ons package if your machine has Internet access, openHAB will download add-ons online as necessary.

```
sudo apt-get install openhab2-addons
```

13.  Navigate with a web browser to  `http://<ip-address>:8080`
14.  Continue by following the  [First-time setup](https://www.openhab.org/docs/tutorial/1sttimesetup.html)  chapter of the  [New User Tutorial](https://www.openhab.org/docs/tutorial/)


### Systems based on sysVinit (e.g. Ubuntu 14.x, Debian Wheezy and older):
```
sudo /etc/init.d/openhab2 start
sudo /etc/init.d/openhab2 status
```
```
sudo update-rc.d openhab2 defaults
```
### Systems based on systemd (e.g. Debian 8, Ubuntu 15.x, Raspbian Jessie and newer):
```
sudo systemctl start openhab2.service
sudo systemctl status openhab2.service

sudo systemctl daemon-reload
sudo systemctl enable openhab2.service
```

>The first start may take ***up to 15 minutes***, this is a good time to reward yourself with hot coffee or a freshly brewed tea!

> You should be able to reach the openHAB 2 Dashboard at http://openhab-device:8080 at this point. If you're new to openHAB, then you should checkout the beginner's tutorial!