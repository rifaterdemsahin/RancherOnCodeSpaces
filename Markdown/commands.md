# Docker install
sudo apt-get update
sudo apt-get upgrade
sudo apt-get -f install
sudo apt-get install containerd
sudo apt-get install -y docker.io
docker --version

@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $   docker --version
Docker version 24.0.7, build 24.0.7-0ubuntu2~20.04.1
@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ 



  docker pull rancher/rancher:latest


  @rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $   docker run -d --restart=unless-stopped -p 80:80 -p 443:443 rancher/rancher
65675e288f67f9018591b6574a7fcc2800de591fd12d257cb5907df084409fc8
@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ DOCKER PS
bash: DOCKER: command not found
@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ docker ps
CONTAINER ID   IMAGE             COMMAND           CREATED          STATUS                         PORTS     NAMES
65675e288f67   rancher/rancher   "entrypoint.sh"   41 seconds ago   Restarting (1) 9 seconds ago             boring_wescoff
@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ 