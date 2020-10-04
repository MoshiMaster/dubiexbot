# Dubiex Discord Bot
This Bot can pull Information from Dubiex.
It's basically a scraping the data directly from Dubiex.

## What you need
A VPS Server. I'm using Vultr for 5$ a month with Debian (Ubuntu works too) installed.
I've also tried making it work with a Raspberry Pi, but some tools sadly don't work with Rasbian OS.

## Guide
**First Steps:**
```sh
adduser username
usermod -aG sudo username
su username
sudo apt-get update
sudo apt-get upgrade -y
sudo apt-get install python3 python3-pip

```
**Installation:**
```sh
# install Python & dependencies
sudo apt-get install python3 python3-dev python3-pip libxml2-dev libxslt1-dev zlib1g-dev libffi-dev libssl-dev
# install Scrapy https://docs.scrapy.org/
pip3 install scrapy
# install Docker
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
sudo docker run hello-world #quick test if docker works
# install Splash Browser via Docker
sudo docker pull scrapinghub/splash
sudo docker run -it -p 8050:8050 --rm scrapinghub/splash # open browser <ip>:8050 
# install Discord.py https://github.com/Rapptz/discord.py
python3 -m pip install -U discord.py
```

more soon
