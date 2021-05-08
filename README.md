# Way 1 

# install Docker on Ubuntu - Орги хувилбар
```bash
sudo apt update  
sudo apt upgrade  
sudo apt install docker.io  
```
# Login as root and setup OJ  
```bash
sudo passwd root  
su -  
cd /home/{your_user}/OnlineJudge  
apt install docker-compose  
docker-compose up -d  
```

# local
```bash
sudo lsof -i tcp:80 -s tcp:listen  
sudo lsof -t -i tcp:80 -s tcp:listen | sudo xargs kill
```

# DONE!!!

pen source online judge based on Vue, Django and Docker. 
青岛大学开源 Online Judge | QQ群 496710125 | admin@qduoj.com 

# Way 2
##  Qingdao-University-OnlineJudge install

 ## Environmental preparation (Linux)

+ System: Ubuntu 18.04 LTS

1. Install the necessary dependencies

    ```bash
    sudo apt-get update
    sudo apt-get install -y vim python3-pip curl git
    pip3 install --upgrade pip
    pip install docker-compose
    ```

2. Install Docker

    Install using script: `sudo curl -sSL get.docker.com | sh`

    Other installation methods: [https://docs.docker.com/install/](https://docs.docker.com/install/)

## Install

1. Please select a location with some surplus disk space and run the following command:

    ```bash
    git clone -b 2.0 https://github.com/QingdaoU/OnlineJudgeDeploy.git && cd OnlineJudgeDeploy
    ```

2. Start service

    ```bash
    docker-compose up -d
    ```

According to the network speed, the setup can be completed automatically in about 5 to 30 minutes without manual intervention.

Wait for the command execution to complete, and then run `docker ps -a`. When you see that the status of all the containers does not have `unhealthy` or `Exited (x) xxx`, it means OnlineJudge has started successfully.

Access the server's HTTP 80 port or HTTPS 443 port through a browser, and you can start using it. The background management path is `/admin`, the super administrator user name automatically added during the installation process is `root`, and the password is `rootroot`. **If you log in successfully, please change your account password immediately.**.

Don't forget to read the documentation: http://docs.onlinejudge.me/
