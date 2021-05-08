## Орги хувилбар
# install Docker on Ubuntu

sudo apt update  
sudo apt upgrade  
sudo apt install docker.io  

# Login as root and setup OJ  

sudo passwd root  
su -  
cd /home/{your_user}/OnlineJudge  
apt install docker-compose  
docker-compose up -d  

# local

sudo lsof -i tcp:80 -s tcp:listen  
sudo lsof -t -i tcp:80 -s tcp:listen | sudo xargs kill


# DONE!!!

pen source online judge based on Vue, Django and Docker. 
青岛大学开源 Online Judge | QQ群 496710125 | admin@qduoj.com 

## Орги хувилбар - Qingdao-University-OnlineJudge
