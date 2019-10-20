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

