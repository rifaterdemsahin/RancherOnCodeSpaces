@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ docker run -d --privileged --restart=unless-stopped -p 80:80 -p 443:443 rancher/rancher
549986bbd36fe1f5eff5b78918c2864f5935e8d7f743a506e6d0bd12c6f66782
@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ docker ps
CONTAINER ID   IMAGE             COMMAND           CREATED         STATUS         PORTS                                                                      NAMES
549986bbd36f   rancher/rancher   "entrypoint.sh"   2 minutes ago   Up 2 minutes   0.0.0.0:80->80/tcp, :::80->80/tcp, 0.0.0.0:443->443/tcp, :::443->443/tcp   peaceful_cerf
@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ docker logs  549986bbd36f  2>&1 | grep "Bootstrap Password:"
2024/10/04 17:30:40 [INFO] Bootstrap Password: 4b9pdk7445l7qz2vvfbsm8nb2t2n98jzmrj9c4rkkvn7mrgs2wd79m
@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ 