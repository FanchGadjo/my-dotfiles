Config machine de dev
===

```
ssh-keygen -b 4096
cat .ssh/id_rsa.pub 
su -
adduser fkerisit sudo
groups
```

```
sudo apt install -y chromium
sudo apt install -y tree git git-flow gitg git-extras
sudo apt install -y default-jre default-jdk
sudo apt -y install unzip
sudo apt -y install wget curl httpie
sudo snap install insomnia
```

Google Chrome :
https://computingforgeeks.com/install-google-chrome-browser-on-debian/

Outils SOAP, REST
```
sudo apt -y install wget curl httpie
sudo snap install insomnia
```

https://computingforgeeks.com/install-netbeans-ide-on-debian-ubuntu-and-linux-mint/
```
cd env/ && wget https://www-us.apache.org/dist/incubator/netbeans/incubating-netbeans/incubating-11.0/incubating-netbeans-11.0-bin.zip 
unzip incubating-netbeans-11.0-bin.zip
ls
sudo mv netbeans/ /opt/
nano ~/.bashrc
source ~/.bashrc
sudo nano /usr/share/applications/netbeans.desktop
display /opt/netbeans/nb/netbeans.png
sudo nano /usr/share/applications/netbeans.desktop
```
NB Plugins : nbjavac Library

```
mkdir proj
cd proj/
ls
cat ~/.ssh/id_rsa.pub 
git clone git@hermod.francead.fr.ad.alphyra.com:developers/invogate-ws.git
cd invogate-ws/
sudo apt -y install docker
```

http://hermod.francead.fr.ad.alphyra.com/tiddlywiki#Artifactory
```
mkdir -pv ~/.m2/
gedit ~/.m2/settings.xml
```

### MySQL
```
sudo apt -y install mariadb-server
sudo mysql
> GRANT ALL PRIVILEGES on *.* to 'root'@'localhost' IDENTIFIED BY '<password>';
> FLUSH PRIVILEGES;
sudo service mysql restart
```
https://computingforgeeks.com/install-phpmyadmin-with-apache-on-debian-10-buster/

https://dev.mysql.com/downloads/workbench/

### Docker
https://docs.docker.com/install/linux/docker-ce/debian/

### Slack
```
sudo apt install snapd
sudo snap install slack --classic
```

### Java 8
https://linuxize.com/post/install-java-on-debian-10/

### Eclipse
https://linuxhint.com/install_eclipse_ide_debian_10/

### NodeJS
https://github.com/nvm-sh/nvm

### Apache
https://www.howtoforge.com/tutorial/ubuntu-apache-gui/

### Gradle
https://gradle.org/install/
avec SDKMan :

https://sdkman.io/

### Ansible
```
echo "#deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main" | sudo tee -a /etc/apt/sources.list
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
sudo apt update
sudo apt install -y ansible
```
https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-ansible-on-debian

```
sudo apt-get install -y python3-pip libssl-dev
python3 -m pip install --user "molecule[lint]"
python3 -m pip install --user "docker-py"
```
https://molecule.readthedocs.io/en/latest/installation.html

### Ruby
Install Ruby through RVM (Ruby Version Manager)

https://rvm.io/

Then run `rvm requirements` on debian to avoid using sudo. Add gen home to dotfile : `export GEM_HOME="$HOME/.gem"`

https://stackoverflow.com/a/53949737/12051588

