ubuntu@ip-10-0-15-89:~$ sudo apt install -y git curl wget unzip nginx
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
git is already the newest version (1:2.43.0-1ubuntu7.3).
git set to manually installed.
wget is already the newest version (1.21.4-1ubuntu4.1).
wget set to manually installed.
The following additional packages will be installed:
  libcurl3t64-gnutls libcurl4t64 nginx-common
Suggested packages:
  fcgiwrap nginx-doc ssl-cert zip
The following NEW packages will be installed:
  nginx nginx-common unzip
The following packages will be upgraded:
  curl libcurl3t64-gnutls libcurl4t64
3 upgraded, 3 newly installed, 0 to remove and 54 not upgraded.
Need to get 1645 kB of archives.
After this operation, 1986 kB of additional disk space will be used.
Get:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 curl amd64 8.5.0-2ubuntu10.9 [227 kB]
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 libcurl4t64 amd64 8.5.0-2ubuntu10.9 [342 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 libcurl3t64-gnutls amd64 8.5.0-2ubuntu10.9 [334 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 nginx-common all 1.24.0-2ubuntu7.11 [44.3 kB]
Get:5 http://us-east-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 nginx amd64 1.24.0-2ubuntu7.11 [523 kB]
Get:6 http://us-east-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 unzip amd64 6.0-28ubuntu4.1 [174 kB]
Fetched 1645 kB in 0s (31.9 MB/s)
Preconfiguring packages ...
(Reading database ... 72559 files and directories currently installed.)
Preparing to unpack .../0-curl_8.5.0-2ubuntu10.9_amd64.deb ...
Unpacking curl (8.5.0-2ubuntu10.9) over (8.5.0-2ubuntu10.8) ...
Preparing to unpack .../1-libcurl4t64_8.5.0-2ubuntu10.9_amd64.deb ...
Unpacking libcurl4t64:amd64 (8.5.0-2ubuntu10.9) over (8.5.0-2ubuntu10.8) ...
Preparing to unpack .../2-libcurl3t64-gnutls_8.5.0-2ubuntu10.9_amd64.deb ...
Unpacking libcurl3t64-gnutls:amd64 (8.5.0-2ubuntu10.9) over (8.5.0-2ubuntu10.8) ...
Selecting previously unselected package nginx-common.
Preparing to unpack .../3-nginx-common_1.24.0-2ubuntu7.11_all.deb ...
Unpacking nginx-common (1.24.0-2ubuntu7.11) ...
Selecting previously unselected package nginx.
Preparing to unpack .../4-nginx_1.24.0-2ubuntu7.11_amd64.deb ...
Unpacking nginx (1.24.0-2ubuntu7.11) ...
Selecting previously unselected package unzip.
Preparing to unpack .../5-unzip_6.0-28ubuntu4.1_amd64.deb ...
Unpacking unzip (6.0-28ubuntu4.1) ...
Setting up libcurl4t64:amd64 (8.5.0-2ubuntu10.9) ...
Setting up unzip (6.0-28ubuntu4.1) ...
Setting up libcurl3t64-gnutls:amd64 (8.5.0-2ubuntu10.9) ...
Setting up nginx-common (1.24.0-2ubuntu7.11) ...
Created symlink /etc/systemd/system/multi-user.target.wants/nginx.service → /usr/lib/systemd/system/nginx.service.
Setting up curl (8.5.0-2ubuntu10.9) ...
Setting up nginx (1.24.0-2ubuntu7.11) ...
 * Upgrading binary nginx                                                                                                                                                                [ OK ]
Processing triggers for ufw (0.36.2-6) ...
Processing triggers for man-db (2.12.0-4build2) ...
Processing triggers for libc-bin (2.39-0ubuntu8.7) ...
Scanning processes...
Scanning linux images...

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
ubuntu@ip-10-0-15-89:~$ curl -fsSL https://get.docker.com | sh
# Executing docker install script, commit: 2687d91ddeb3bd6aeae37a90947761efdee87030
+ sudo -E sh -c apt-get -qq update >/dev/null
+ sudo -E sh -c DEBIAN_FRONTEND=noninteractive apt-get -y -qq install ca-certificates curl >/dev/null
+ sudo -E sh -c install -m 0755 -d /etc/apt/keyrings
+ sudo -E sh -c curl -fsSL "https://download.docker.com/linux/ubuntu/gpg" -o /etc/apt/keyrings/docker.asc
+ sudo -E sh -c chmod a+r /etc/apt/keyrings/docker.asc
+ sudo -E sh -c echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu noble stable" > /etc/apt/sources.list.d/docker.list
+ sudo -E sh -c apt-get -qq update >/dev/null
+ sudo -E sh -c DEBIAN_FRONTEND=noninteractive apt-get -y -qq install docker-ce docker-ce-cli containerd.io docker-compose-plugin docker-ce-rootless-extras docker-buildx-plugin docker-model-plugin >/dev/null
Scanning processes...
Scanning linux images...
Using systemd to manage Docker service
+ sudo -E sh -c systemctl enable --now docker.service 2>/dev/null
INFO: Docker daemon enabled and started

+ sudo -E sh -c docker version
Client: Docker Engine - Community
 Version:           29.5.3
 API version:       1.54
 Go version:        go1.26.4
 Git commit:        d1c06ef
 Built:             Wed Jun  3 18:00:12 2026
 OS/Arch:           linux/amd64
 Context:           default

Server: Docker Engine - Community
 Engine:
  Version:          29.5.3
  API version:      1.54 (minimum version 1.40)
  Go version:       go1.26.4
  Git commit:       285b471
  Built:            Wed Jun  3 18:00:12 2026
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          v2.2.4
  GitCommit:        193637f7ee8ae5f5aa5248f49e7baa3e6164966e
 runc:
  Version:          1.3.5
  GitCommit:        v1.3.5-0-g488fc13e
 docker-init:
  Version:          0.19.0
  GitCommit:        de40ad0

================================================================================

To run Docker as a non-privileged user, consider setting up the
Docker daemon in rootless mode for your user:

    dockerd-rootless-setuptool.sh install

Visit https://docs.docker.com/go/rootless/ to learn about rootless mode.


To run the Docker daemon as a fully privileged service, but granting non-root
users access, refer to https://docs.docker.com/go/daemon-access/

WARNING: Access to the remote API on a privileged Docker daemon is equivalent
         to root access on the host. Refer to the 'Docker daemon attack surface'
         documentation for details: https://docs.docker.com/go/attack-surface/

================================================================================

ubuntu@ip-10-0-15-89:~$ sudo usermod -aG docker ubuntu
ubuntu@ip-10-0-15-89:~$ newgrp docker
ubuntu@ip-10-0-15-89:~$ docker --version
Docker version 29.5.3, build d1c06ef
ubuntu@ip-10-0-15-89:~$
ubuntu@ip-10-0-15-89:~$ sudo apt install docker-compose-plugin -y
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
docker-compose-plugin is already the newest version (5.1.4-1~ubuntu.24.04~noble).
0 upgraded, 0 newly installed, 0 to remove and 54 not upgraded.
ubuntu@ip-10-0-15-89:~$ docker compose version
Docker Compose version v5.1.4
ubuntu@ip-10-0-15-89:~$


ubuntu@ip-10-0-15-89:~$ cd ~
ubuntu@ip-10-0-15-89:~$ git clone https://github.com/shajedultonmoy/Assignment-on-module-8.git
Cloning into 'Assignment-on-module-8'...
remote: Enumerating objects: 11802, done.
remote: Counting objects: 100% (11802/11802), done.
remote: Compressing objects: 100% (8156/8156), done.
remote: Total 11802 (delta 3298), reused 11802 (delta 3298), pack-reused 0 (from 0)
Receiving objects: 100% (11802/11802), 26.62 MiB | 23.62 MiB/s, done.
Resolving deltas: 100% (3298/3298), done.
ubuntu@ip-10-0-15-89:~$ cd Assignment-on-module-8
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ cd backend
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8/backend$ nano Dockerfile
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8/backend$ cd ../frontend
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8/frontend$ nano Dockerfile
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8/frontend$ cd ..
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ nano docker-compose.yml
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ docker compose up -d --build
[+] Building 56.1s (20/20) FINISHED
 => [internal] load local bake definitions                                                                                                                                                 0.0s
 => => reading from stdin 1.06kB                                                                                                                                                           0.0s
 => [backend internal] load build definition from Dockerfile                                                                                                                               0.0s
 => => transferring dockerfile: 153B                                                                                                                                                       0.0s
 => [frontend internal] load build definition from Dockerfile                                                                                                                              0.1s
 => => transferring dockerfile: 168B                                                                                                                                                       0.0s
 => [frontend internal] load metadata for docker.io/library/node:20                                                                                                                        0.4s
 => [backend internal] load .dockerignore                                                                                                                                                  0.0s
 => => transferring context: 2B                                                                                                                                                            0.0s
 => [frontend internal] load .dockerignore                                                                                                                                                 0.0s
 => => transferring context: 2B                                                                                                                                                            0.0s
 => [backend 1/5] FROM docker.io/library/node:20@sha256:8f693eaa7e0a8e71560c9a82b55fd54c2ae920a2ba5d2cde28bac7d1c01c9ba5                                                                  19.9s
 => => resolve docker.io/library/node:20@sha256:8f693eaa7e0a8e71560c9a82b55fd54c2ae920a2ba5d2cde28bac7d1c01c9ba5                                                                           0.1s
 => => sha256:0b22ec2d9b1a1a0e906e301b5ef08efe7774d5fc001b9cfa08e4e980152a0357 448B / 448B                                                                                                 0.1s
 => => sha256:2f2ab6e4eb4619f7b8506c38dc79c8adf77acffb7622bc15ceeabb0fbc73b8a1 1.25MB / 1.25MB                                                                                             0.6s
 => => sha256:76e6b8204a89d20e7915fdc9a98ff33cb65fd7ce44ecf5a84b6cfca4bdb3d6d0 48.62MB / 48.62MB                                                                                           3.7s
 => => sha256:c83419f4430962505175b565eb8a24aafeaa4d441c0b22234e94c6e8160848ba 3.32kB / 3.32kB                                                                                             0.1s
 => => sha256:8fcda2b4d7993820b00c5488d173051e76d01ba6b85620617ba77001b0f9e2fa 64.40MB / 64.40MB                                                                                           4.0s
 => => sha256:2933ecab0f11302fd71f29aa83ad2904683246f7a8320ad0dc3a60b23f05fee9 211.55MB / 211.55MB                                                                                         5.7s
 => => sha256:e5203b2bfeff92b72e816dc6cbb1f16856f0cd592e521e3c0cfa195a78fe180e 24.04MB / 24.04MB                                                                                           2.4s
 => => sha256:db53381ee51f9e43304e236099ba097ae1b33ae41a8007e0b6319992eb55fd00 48.49MB / 48.49MB                                                                                           1.3s
 => => extracting sha256:db53381ee51f9e43304e236099ba097ae1b33ae41a8007e0b6319992eb55fd00                                                                                                  2.3s
 => => extracting sha256:e5203b2bfeff92b72e816dc6cbb1f16856f0cd592e521e3c0cfa195a78fe180e                                                                                                  0.6s
 => => extracting sha256:8fcda2b4d7993820b00c5488d173051e76d01ba6b85620617ba77001b0f9e2fa                                                                                                  2.4s
 => => extracting sha256:2933ecab0f11302fd71f29aa83ad2904683246f7a8320ad0dc3a60b23f05fee9                                                                                                  6.4s
 => => extracting sha256:c83419f4430962505175b565eb8a24aafeaa4d441c0b22234e94c6e8160848ba                                                                                                  0.0s
 => => extracting sha256:76e6b8204a89d20e7915fdc9a98ff33cb65fd7ce44ecf5a84b6cfca4bdb3d6d0                                                                                                  2.8s
 => => extracting sha256:2f2ab6e4eb4619f7b8506c38dc79c8adf77acffb7622bc15ceeabb0fbc73b8a1                                                                                                  0.2s
 => => extracting sha256:0b22ec2d9b1a1a0e906e301b5ef08efe7774d5fc001b9cfa08e4e980152a0357                                                                                                  0.1s
 => [backend internal] load build context                                                                                                                                                  3.1s
 => => transferring context: 36.52MB                                                                                                                                                       3.0s
 => [frontend internal] load build context                                                                                                                                                 4.0s
 => => transferring context: 81.10MB                                                                                                                                                       3.9s
 => [backend 2/5] WORKDIR /app                                                                                                                                                             1.5s
 => [frontend 3/5] COPY package*.json ./                                                                                                                                                   0.1s
 => [backend 3/5] COPY package*.json ./                                                                                                                                                    0.1s
 => [backend 4/5] RUN npm install                                                                                                                                                          9.3s
 => [frontend 4/5] RUN npm install                                                                                                                                                        11.7s
 => [backend 5/5] COPY . .                                                                                                                                                                 3.0s
 => [frontend 5/5] COPY . .                                                                                                                                                                5.0s
 => [backend] exporting to image                                                                                                                                                           9.0s
 => => exporting layers                                                                                                                                                                    5.1s
 => => exporting manifest sha256:ef5238b2216013b0d41f2dc5f51e3e26b82c5978383e86a02e30d0d5fb6b3ab3                                                                                          0.0s
 => => exporting config sha256:192b3b5e8fd184785df2dc7e96895660b3eb7b43ec3a48805c85f5f8795c0e88                                                                                            0.0s
 => => exporting attestation manifest sha256:9508da5bf63d3f4e3ea999d3ada2c99b109ceb82eee07fbed70342ea35647071                                                                              0.0s
 => => exporting manifest list sha256:67c13b113039c57184e7f56bbc9160aec422bb90ce9d92ebbcb614214185feaf                                                                                     0.0s
 => => naming to docker.io/library/assignment-on-module-8-backend:latest                                                                                                                   0.0s
 => => unpacking to docker.io/library/assignment-on-module-8-backend:latest                                                                                                                3.6s
 => [frontend] exporting to image                                                                                                                                                         17.1s
 => => exporting layers                                                                                                                                                                   13.2s
 => => exporting manifest sha256:b695333a1712981faffb35b2b4cbb04341fb17e479c29e9b24b1b33f78583a14                                                                                          0.0s
 => => exporting config sha256:6785d5c88e6337954f76cceb9664fb785442c460768d1cfe2bafac1c3874f2ef                                                                                            0.0s
 => => exporting attestation manifest sha256:5d0ccfd4bc1a6fb220c17586c8ade51cb632b628701769844b185b6bd00de443                                                                              0.0s
 => => exporting manifest list sha256:25af985ae6caf4a4eb79f08eb56796674e9b9832e7c8a1dce791c0824bc18226                                                                                     0.0s
 => => naming to docker.io/library/assignment-on-module-8-frontend:latest                                                                                                                  0.0s
 => => unpacking to docker.io/library/assignment-on-module-8-frontend:latest                                                                                                               3.7s
 => [backend] resolving provenance for metadata file                                                                                                                                       0.1s
 => [frontend] resolving provenance for metadata file                                                                                                                                      0.0s
[+] up 5/5
 ✔ Image assignment-on-module-8-backend   Built                                                                                                                                            56.2s
 ✔ Image assignment-on-module-8-frontend  Built                                                                                                                                            56.2s
 ✔ Network assignment-on-module-8_default Created                                                                                                                                           0.1s
 ✔ Container hospital-backend             Started                                                                                                                                           1.2s
 ✔ Container hospital-frontend            Started                                                                                                                                           1.2s
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ docker ps
CONTAINER ID   IMAGE                             COMMAND                  CREATED          STATUS                          PORTS     NAMES
24f22679cecb   assignment-on-module-8-backend    "docker-entrypoint.s…"   32 seconds ago   Restarting (1) 11 seconds ago             hospital-backend
bff4497225e0   assignment-on-module-8-frontend   "docker-entrypoint.s…"   32 seconds ago   Restarting (127) 1 second ago             hospital-frontend
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$



ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo nano /etc/nginx/sites-available/hospital
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo ln -s /etc/nginx/sites-available/hospital /etc/nginx/sites-enabled/
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo nginx -t
2026/06/10 14:39:19 [warn] 6562#6562: conflicting server name "_" on 0.0.0.0:80, ignored
nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
nginx: configuration file /etc/nginx/nginx.conf test is successful
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo systemctl restart nginx
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$


ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo nano /etc/nginx/sites-available/hospital
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo ln -s /etc/nginx/sites-available/hospital /etc/nginx/sites-enabled/
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo nginx -t
2026/06/10 14:39:19 [warn] 6562#6562: conflicting server name "_" on 0.0.0.0:80, ignored
nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
nginx: configuration file /etc/nginx/nginx.conf test is successful
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo systemctl restart nginx
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ cat ~/.ssh/id_rsa
cat: /home/ubuntu/.ssh/id_rsa: No such file or directory
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ ssh-keygen -t rsa -b 4096
Generating public/private rsa key pair.
Enter file in which to save the key (/home/ubuntu/.ssh/id_rsa): ubuntu
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in ubuntu
Your public key has been saved in ubuntu.pub
The key fingerprint is:
SHA256:rosSlLNyrawoOo122iqt7w5g7KKbTOI7Q6OkHZP0yfY ubuntu@ip-10-0-15-89
The key's randomart image is:
+---[RSA 4096]----+
|                 |
|                 |
|   .             |
|. =              |
|.= B .  S        |
|=+B *  .         |
|O@.* .  .        |
|/*O. .E.         |
|&#@o. o.         |
+----[SHA256]-----+


ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ mkdir monitoring
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ cd monitoring
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8/monitoring$ nano prometheus.yml
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8/monitoring$ cd ~
ubuntu@ip-10-0-15-89:~$
ubuntu@ip-10-0-15-89:~$ wget https://github.com/prometheus/node_exporter/releases/latest/download/node_exporter-1.9.1.linux-amd64.tar.gz
--2026-06-10 15:15:47--  https://github.com/prometheus/node_exporter/releases/latest/download/node_exporter-1.9.1.linux-amd64.tar.gz
Resolving github.com (github.com)... 140.82.113.4
Connecting to github.com (github.com)|140.82.113.4|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://github.com/prometheus/node_exporter/releases/download/v1.11.1/node_exporter-1.9.1.linux-amd64.tar.gz [following]
--2026-06-10 15:15:47--  https://github.com/prometheus/node_exporter/releases/download/v1.11.1/node_exporter-1.9.1.linux-amd64.tar.gz
Reusing existing connection to github.com:443.
HTTP request sent, awaiting response... 404 Not Found
2026-06-10 15:15:48 ERROR 404: Not Found.

ubuntu@ip-10-0-15-89:~$ tar xvf node_exporter-*.tar.gz
tar: node_exporter-*.tar.gz: Cannot open: No such file or directory
tar: Error is not recoverable: exiting now
ubuntu@ip-10-0-15-89:~$ wget https://github.com/prometheus/node_exporter/releases/download/v1.11.1/node_exporter-1.11.1.linux-amd64.tar.gz
--2026-06-10 15:17:04--  https://github.com/prometheus/node_exporter/releases/download/v1.11.1/node_exporter-1.11.1.linux-amd64.tar.gz
Resolving github.com (github.com)... 140.82.112.4
Connecting to github.com (github.com)|140.82.112.4|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://release-assets.githubusercontent.com/github-production-release-asset/9524057/fae42cf1-aefe-4590-b9ee-e8cd71d69ffc?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-06-10T16%3A15%3A36Z&rscd=attachment%3B+filename%3Dnode_exporter-1.11.1.linux-amd64.tar.gz&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-06-10T15%3A15%3A00Z&ske=2026-06-10T16%3A15%3A36Z&sks=b&skv=2018-11-09&sig=%2BhQ1xbhBtBA9f%2BEQnczFMMg5Yf40l4tzo2cmpUqn%2B7Y%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc4MTEwNjQyNCwibmJmIjoxNzgxMTA0NjI0LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.GrK-7gJly9g5VmcoyhcNNe1EbmslIJHT6mq_gGux_Ww&response-content-disposition=attachment%3B%20filename%3Dnode_exporter-1.11.1.linux-amd64.tar.gz&response-content-type=application%2Foctet-stream [following]
--2026-06-10 15:17:04--  https://release-assets.githubusercontent.com/github-production-release-asset/9524057/fae42cf1-aefe-4590-b9ee-e8cd71d69ffc?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-06-10T16%3A15%3A36Z&rscd=attachment%3B+filename%3Dnode_exporter-1.11.1.linux-amd64.tar.gz&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-06-10T15%3A15%3A00Z&ske=2026-06-10T16%3A15%3A36Z&sks=b&skv=2018-11-09&sig=%2BhQ1xbhBtBA9f%2BEQnczFMMg5Yf40l4tzo2cmpUqn%2B7Y%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc4MTEwNjQyNCwibmJmIjoxNzgxMTA0NjI0LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.GrK-7gJly9g5VmcoyhcNNe1EbmslIJHT6mq_gGux_Ww&response-content-disposition=attachment%3B%20filename%3Dnode_exporter-1.11.1.linux-amd64.tar.gz&response-content-type=application%2Foctet-stream
Resolving release-assets.githubusercontent.com (release-assets.githubusercontent.com)... 185.199.111.133, 185.199.108.133, 185.199.109.133, ...
Connecting to release-assets.githubusercontent.com (release-assets.githubusercontent.com)|185.199.111.133|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 12084398 (12M) [application/octet-stream]
Saving to: ‘node_exporter-1.11.1.linux-amd64.tar.gz’

node_exporter-1.11.1.linux-amd64.tar.gz         100%[=======================================================================================================>]  11.52M  --.-KB/s    in 0.03s

2026-06-10 15:17:04 (368 MB/s) - ‘node_exporter-1.11.1.linux-amd64.tar.gz’ saved [12084398/12084398]

ubuntu@ip-10-0-15-89:~$ tar xvf node_exporter-1.11.1.linux-amd64.tar.gz
node_exporter-1.11.1.linux-amd64/
node_exporter-1.11.1.linux-amd64/LICENSE
node_exporter-1.11.1.linux-amd64/node_exporter
node_exporter-1.11.1.linux-amd64/NOTICE
ubuntu@ip-10-0-15-89:~$ sudo mv node_exporter-*/node_exporter /usr/local/bin/
ubuntu@ip-10-0-15-89:~$ sudo nano /etc/systemd/system/node_exporter.service
ubuntu@ip-10-0-15-89:~$ sudo systemctl daemon-reload
ubuntu@ip-10-0-15-89:~$ sudo systemctl enable node_exporter
Created symlink /etc/systemd/system/multi-user.target.wants/node_exporter.service → /etc/systemd/system/node_exporter.service.
ubuntu@ip-10-0-15-89:~$ sudo systemctl start node_exporter
ubuntu@ip-10-0-15-89:~$

ubuntu@ip-10-0-15-89:~$ nano docker-compose.yml
ubuntu@ip-10-0-15-89:~$ docker compose up -d
[+] up 12/13
 ✔ Image prom/prometheus  Pulled                                                                                                                                                            6.1s
 ✔ Network ubuntu_default Created                                                                                                                                                           0.1s
 ⠼ Container prometheus   Starting                                                                                                                                                          1.4s
Error response from daemon: failed to create task for container: failed to create shim task: OCI runtime create failed: runc create failed: unable to start container process: error during container init: error mounting "/home/ubuntu/prometheus.yml" to rootfs at "/etc/prometheus/prometheus.yml": mount src=/home/ubuntu/prometheus.yml, dst=/etc/prometheus/prometheus.yml, dstFd=/proc/thread-self/fd/11, flags=MS_BIND|MS_REC: not a directory: Are you trying to mount a directory onto a file (or vice-versa)? Check if the specified host path exists and is the expected type
ubuntu@ip-10-0-15-89:~$



ubuntu@ip-10-0-15-89:~$ docker compose up -d
[+] up 0/1
 ⠙ Container prometheus Starting                                                                                                                                                            0.1s
Error response from daemon: failed to create task for container: failed to create shim task: OCI runtime create failed: runc create failed: unable to start container process: error during container init: error mounting "/home/ubuntu/prometheus.yml" to rootfs at "/etc/prometheus/prometheus.yml": mount src=/home/ubuntu/prometheus.yml, dst=/etc/prometheus/prometheus.yml, dstFd=/proc/thread-self/fd/11, flags=MS_BIND|MS_REC: not a directory: Are you trying to mount a directory onto a file (or vice-versa)? Check if the specified host path exists and is the expected type
ubuntu@ip-10-0-15-89:~$ file /home/ubuntu/prometheus.yml
/home/ubuntu/prometheus.yml: directory
ubuntu@ip-10-0-15-89:~$ rm -rf /home/ubuntu/prometheus.yml
ubuntu@ip-10-0-15-89:~$ docker compose down
[+] down 2/2
 ✔ Container prometheus   Removed                                                                                                                                                           0.0s
 ✔ Network ubuntu_default Removed                                                                                                                                                           0.1s
ubuntu@ip-10-0-15-89:~$ docker compose up -d
[+] up 1/2
 ✔ Network ubuntu_default Created                                                                                                                                                           0.1s
 ⠹ Container prometheus   Starting                                                                                                                                                          0.3s
Error response from daemon: failed to create task for container: failed to create shim task: OCI runtime create failed: runc create failed: unable to start container process: error during container init: error mounting "/home/ubuntu/prometheus.yml" to rootfs at "/etc/prometheus/prometheus.yml": mount src=/home/ubuntu/prometheus.yml, dst=/etc/prometheus/prometheus.yml, dstFd=/proc/thread-self/fd/11, flags=MS_BIND|MS_REC: not a directory: Are you trying to mount a directory onto a file (or vice-versa)? Check if the specified host path exists and is the expected type
ubuntu@ip-10-0-15-89:~$ docker ps
CONTAINER ID   IMAGE                             COMMAND                  CREATED          STATUS                                    PORTS     NAMES
24f22679cecb   assignment-on-module-8-backend    "docker-entrypoint.s…"   49 minutes ago   Restarting (1) 51 seconds ago                       hospital-backend
bff4497225e0   assignment-on-module-8-frontend   "docker-entrypoint.s…"   49 minutes ago   Restarting (127) Less than a second ago             hospital-frontend
ubuntu@ip-10-0-15-89:~$ docker logs prometheus
ubuntu@ip-10-0-15-89:~$ ls -ld /home/ubuntu/prometheus.yml
drwxr-xr-x 2 root root 4096 Jun 10 15:26 /home/ubuntu/prometheus.yml
ubuntu@ip-10-0-15-89:~$ nano /home/ubuntu/prometheus.yml
ubuntu@ip-10-0-15-89:~$
ubuntu@ip-10-0-15-89:~$ sudo cat > /home/ubuntu/prometheus.yml << 'EOF'
global:
  scrape_interval: 15s

scrape_configs:
  - job_name: node
    static_configs:
      - targets:
        - localhost:9100
EOF
bash: /home/ubuntu/prometheus.yml: Is a directory
ubuntu@ip-10-0-15-89:~$ cat /home/ubuntu/prometheus.yml
cat: /home/ubuntu/prometheus.yml: Is a directory
ubuntu@ip-10-0-15-89:~$ file /home/ubuntu/prometheus.yml
/home/ubuntu/prometheus.yml: directory
ubuntu@ip-10-0-15-89:~$ cat docker-compose.yml
services:

  prometheus:
    image: prom/prometheus
    container_name: prometheus

    ports:
      - "9090:9090"

    volumes:
      - ./prometheus.yml:/etc/prometheus/prometheus.yml
ubuntu@ip-10-0-15-89:~$ docker compose down
[+] down 2/2
 ✔ Container prometheus   Removed                                                                                                                                                           0.0s
 ✔ Network ubuntu_default Removed                                                                                                                                                           0.1s
ubuntu@ip-10-0-15-89:~$ docker compose up -d
[+] up 1/2
 ✔ Network ubuntu_default Created                                                                                                                                                           0.1s
 ⠹ Container prometheus   Starting                                                                                                                                                          0.2s
Error response from daemon: failed to create task for container: failed to create shim task: OCI runtime create failed: runc create failed: unable to start container process: error during container init: error mounting "/home/ubuntu/prometheus.yml" to rootfs at "/etc/prometheus/prometheus.yml": mount src=/home/ubuntu/prometheus.yml, dst=/etc/prometheus/prometheus.yml, dstFd=/proc/thread-self/fd/11, flags=MS_BIND|MS_REC: not a directory: Are you trying to mount a directory onto a file (or vice-versa)? Check if the specified host path exists and is the expected type
ubuntu@ip-10-0-15-89:~$ sudo rm -rf /home/ubuntu/prometheus.yml
ubuntu@ip-10-0-15-89:~$ ls -ld /home/ubuntu/prometheus.yml
ls: cannot access '/home/ubuntu/prometheus.yml': No such file or directory
ubuntu@ip-10-0-15-89:~$ cat > /home/ubuntu/prometheus.yml <<EOF
global:
  scrape_interval: 15s

scrape_configs:
  - job_name: node
    static_configs:
      - targets:
          - localhost:9100
EOF
ubuntu@ip-10-0-15-89:~$ file /home/ubuntu/prometheus.yml
/home/ubuntu/prometheus.yml: ASCII text
ubuntu@ip-10-0-15-89:~$ cat /home/ubuntu/prometheus.yml
global:
  scrape_interval: 15s

scrape_configs:
  - job_name: node
    static_configs:
      - targets:
          - localhost:9100
ubuntu@ip-10-0-15-89:~$ docker compose down
[+] down 2/2
 ✔ Container prometheus   Removed                                                                                                                                                           0.0s
 ✔ Network ubuntu_default Removed                                                                                                                                                           0.1s
ubuntu@ip-10-0-15-89:~$ docker compose up -d
[+] up 2/2
 ✔ Network ubuntu_default Created                                                                                                                                                           0.1s
 ✔ Container prometheus   Started                                                                                                                                                           0.3s
ubuntu@ip-10-0-15-89:~$ docker ps
CONTAINER ID   IMAGE                             COMMAND                  CREATED             STATUS                            PORTS                                         NAMES
5f4568a39c0d   prom/prometheus                   "/bin/prometheus --c…"   10 seconds ago      Up 9 seconds                      0.0.0.0:9090->9090/tcp, [::]:9090->9090/tcp   prometheus
24f22679cecb   assignment-on-module-8-backend    "docker-entrypoint.s…"   About an hour ago   Restarting (1) 40 seconds ago                                                   hospital-backend
bff4497225e0   assignment-on-module-8-frontend   "docker-entrypoint.s…"   About an hour ago   Restarting (127) 51 seconds ago                                                 hospital-frontend
ubuntu@ip-10-0-15-89:~$



ubuntu@ip-10-0-15-89:~$ mkdir grafana-stack
ubuntu@ip-10-0-15-89:~$ cd grafana-stack
ubuntu@ip-10-0-15-89:~/grafana-stack$ nano docker-compose.yml
ubuntu@ip-10-0-15-89:~/grafana-stack$ docker compose up -d
[+] up 40/40
 ✔ Image grafana/loki:latest          Pulled                                                                                                                                                9.0s
 ✔ Image grafana/grafana:latest       Pulled                                                                                                                                               21.6s
 ✔ Image grafana/promtail:latest      Pulled                                                                                                                                               10.2s
 ✔ Network grafana-stack_default      Created                                                                                                                                               0.1s
 ✔ Container grafana-stack-loki-1     Started                                                                                                                                               1.5s
 ✔ Container grafana-stack-promtail-1 Started                                                                                                                                               1.5s
 ✔ Container grafana-stack-grafana-1  Started                                                                                                                                               1.4s
ubuntu@ip-10-0-15-89:~/grafana-stack$



ubuntu@ip-10-0-15-89:~/grafana-stack$ docker ps | grep node
ubuntu@ip-10-0-15-89:~/grafana-stack$ docker run -d \
  --name node-exporter \
  --network assignment-on-module-8_default \
  -p 9100:9100 \
  prom/node-exporter:latest
Unable to find image 'prom/node-exporter:latest' locally
latest: Pulling from prom/node-exporter
fe82e83000f4: Pull complete
a6680b927350: Pull complete
a2243411ec8e: Pull complete
Digest: sha256:e9cff4fc67b1818f8c97adb115b9f12c9a54b533de86765d4a0effc01b357205
Status: Downloaded newer image for prom/node-exporter:latest
949c7518f9abc56a4a9863a8c188076399ae4b2ebe3897585aa7e3a8f42c12ed
docker: Error response from daemon: failed to set up container networking: driver failed programming external connectivity on endpoint node-exporter (93ebdcbf6aedcfa22586eaaed5a8e84901cd208b262fde156187365305bf4d77): failed to bind host port 0.0.0.0:9100/tcp: address already in use

Run 'docker run --help' for more information
ubuntu@ip-10-0-15-89:~/grafana-stack$ curl http://localhost:9100/metrics | head -10
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0# HELP go_gc_duration_seconds A summary of the wall-time pause (stop-the-world) duration in garbage collection cycles.
# TYPE go_gc_duration_seconds summary
go_gc_duration_seconds{quantile="0"} 2.4852e-05
go_gc_duration_seconds{quantile="0.25"} 3.4299e-05
go_gc_duration_seconds{quantile="0.5"} 3.6631e-05
go_gc_duration_seconds{quantile="0.75"} 3.8829e-05
go_gc_duration_seconds{quantile="1"} 4.8902e-05
go_gc_duration_seconds_sum 0.000855833
go_gc_duration_seconds_count 23
# HELP go_gc_gogc_percent Heap size target percentage configured by the user, otherwise 100. This value is set by the GOGC environment variable, and the runtime/debug.SetGCPercent function. Sourced from /gc/gogc:percent.
100 20480    0 20480    0     0   699k      0 --:--:-- --:--:-- --:--:--  714k
curl: (23) Failure writing output to destination
ubuntu@ip-10-0-15-89:~/grafana-stack$ docker exec -it $(docker ps | grep prometheus | awk '{print $1}') sh
/prometheus $
/prometheus $
/prometheus $ wget -O- http://node-exporter:9100/metrics | head -10
wget: bad address 'node-exporter:9100'
/prometheus $ exit
ubuntu@ip-10-0-15-89:~/grafana-stack$ curl http://localhost:9090/api/v1/targets | grep -A5 "node"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   677  100   677    0     0  39466      0 --:--:-- --:--:-- --:--:-- 39823
{"status":"success","data":{"activeTargets":[{"discoveredLabels":{"__address__":"localhost:9100","__metrics_path__":"/metrics","__scheme__":"http","__scrape_interval__":"15s","__scrape_timeout__":"10s","job":"node"},"labels":{"instance":"localhost:9100","job":"node"},"scrapePool":"node","scrapeUrl":"http://localhost:9100/metrics","globalUrl":"http://5f4568a39c0d:9100/metrics","lastError":"Get \"http://localhost:9100/metrics\": dial tcp [::1]:9100: connect: connection refused","lastScrape":"2026-06-10T16:04:50.029085707Z","lastScrapeDuration":0.000646421,"health":"down","scrapeInterval":"15s","scrapeTimeout":"10s"}],"droppedTargets":[],"droppedTargetCounts":{"node":0}}}
ubuntu@ip-10-0-15-89:~/grafana-stack$ cat /home/ubuntu/prometheus.yml
global:
  scrape_interval: 15s

scrape_configs:
  - job_name: node
    static_configs:
      - targets:
          - localhost:9100
ubuntu@ip-10-0-15-89:~/grafana-stack$ sudo nano /home/ubuntu/prometheus.yml
ubuntu@ip-10-0-15-89:~/grafana-stack$ cd ~/Assignment-on-module-8
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ docker compose down
[+] down 3/3
 ✔ Container hospital-backend             Removed                                                                                                                                           0.1s
 ✔ Container hospital-frontend            Removed                                                                                                                                           0.1s
 ✔ Network assignment-on-module-8_default Removed                                                                                                                                           0.1s
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ docker compose up -d
[+] up 3/3
 ✔ Network assignment-on-module-8_default Created                                                                                                                                           0.1s
 ✔ Container hospital-backend             Started                                                                                                                                           0.4s
 ✔ Container hospital-frontend            Started                                                                                                                                           0.5s
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ docker ps
CONTAINER ID   IMAGE                             COMMAND                  CREATED          STATUS                           PORTS                                         NAMES
02fcb89f968b   assignment-on-module-8-backend    "docker-entrypoint.s…"   9 seconds ago    Restarting (1) 1 second ago                                                    hospital-backend
85467fd1f442   assignment-on-module-8-frontend   "docker-entrypoint.s…"   9 seconds ago    Restarting (127) 2 seconds ago                                                 hospital-frontend
2c8748e9fd2c   grafana/loki:latest               "/usr/bin/loki -conf…"   21 minutes ago   Up 21 minutes                    0.0.0.0:3100->3100/tcp, [::]:3100->3100/tcp   grafana-stack-loki-1
dc484fdc1fd8   grafana/grafana:latest            "/run.sh"                21 minutes ago   Up 21 minutes                    0.0.0.0:3000->3000/tcp, [::]:3000->3000/tcp   grafana-stack-grafana-1
cd2adc361f55   grafana/promtail:latest           "/usr/bin/promtail -…"   21 minutes ago   Up 21 minutes                                                                  grafana-stack-promtail-1
5f4568a39c0d   prom/prometheus                   "/bin/prometheus --c…"   28 minutes ago   Up 28 minutes                    0.0.0.0:9090->9090/tcp, [::]:9090->9090/tcp   prometheus
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$


ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ docker stop node-exporter
node-exporter
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ docker rm node-exporter
node-exporter
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ sudo nano /home/ubuntu/grafana-stack/prometheus.yml
ubuntu@ip-10-0-15-89:~/Assignment-on-module-8$ cd /tmp
ubuntu@ip-10-0-15-89:/tmp$ wget https://github.com/prometheus/node_exporter/releases/download/v1.11.1/node_exporter-1.11.1.linux-amd64.tar.gz
--2026-06-10 16:11:25--  https://github.com/prometheus/node_exporter/releases/download/v1.11.1/node_exporter-1.11.1.linux-amd64.tar.gz
Resolving github.com (github.com)... 140.82.113.3
Connecting to github.com (github.com)|140.82.113.3|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://release-assets.githubusercontent.com/github-production-release-asset/9524057/fae42cf1-aefe-4590-b9ee-e8cd71d69ffc?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-06-10T16%3A54%3A13Z&rscd=attachment%3B+filename%3Dnode_exporter-1.11.1.linux-amd64.tar.gz&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-06-10T15%3A54%3A03Z&ske=2026-06-10T16%3A54%3A13Z&sks=b&skv=2018-11-09&sig=1ScAhDAyYvfCC7%2FXP1eTm9cRFoQvH2RA0zYgQDvNW6s%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc4MTEwOTY4NSwibmJmIjoxNzgxMTA3ODg1LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.3g152PPIVBIL1rG0cHBijt7EQ0epHG_nu6WjI_0avHw&response-content-disposition=attachment%3B%20filename%3Dnode_exporter-1.11.1.linux-amd64.tar.gz&response-content-type=application%2Foctet-stream [following]
--2026-06-10 16:11:25--  https://release-assets.githubusercontent.com/github-production-release-asset/9524057/fae42cf1-aefe-4590-b9ee-e8cd71d69ffc?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-06-10T16%3A54%3A13Z&rscd=attachment%3B+filename%3Dnode_exporter-1.11.1.linux-amd64.tar.gz&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-06-10T15%3A54%3A03Z&ske=2026-06-10T16%3A54%3A13Z&sks=b&skv=2018-11-09&sig=1ScAhDAyYvfCC7%2FXP1eTm9cRFoQvH2RA0zYgQDvNW6s%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc4MTEwOTY4NSwibmJmIjoxNzgxMTA3ODg1LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.3g152PPIVBIL1rG0cHBijt7EQ0epHG_nu6WjI_0avHw&response-content-disposition=attachment%3B%20filename%3Dnode_exporter-1.11.1.linux-amd64.tar.gz&response-content-type=application%2Foctet-stream
Resolving release-assets.githubusercontent.com (release-assets.githubusercontent.com)... 185.199.111.133, 185.199.110.133, 185.199.109.133, ...
Connecting to release-assets.githubusercontent.com (release-assets.githubusercontent.com)|185.199.111.133|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 12084398 (12M) [application/octet-stream]
Saving to: ‘node_exporter-1.11.1.linux-amd64.tar.gz’

node_exporter-1.11.1.linux-amd64.tar.gz         100%[=======================================================================================================>]  11.52M  --.-KB/s    in 0.04s

2026-06-10 16:11:25 (286 MB/s) - ‘node_exporter-1.11.1.linux-amd64.tar.gz’ saved [12084398/12084398]

ubuntu@ip-10-0-15-89:/tmp$ tar xvf node_exporter-1.11.1.linux-amd64.tar.gz
node_exporter-1.11.1.linux-amd64/
node_exporter-1.11.1.linux-amd64/LICENSE
node_exporter-1.11.1.linux-amd64/node_exporter
node_exporter-1.11.1.linux-amd64/NOTICE
ubuntu@ip-10-0-15-89:/tmp$ sudo mv node_exporter-1.11.1.linux-amd64/node_exporter /usr/local/bin/
ubuntu@ip-10-0-15-89:/tmp$ sudo tee /etc/systemd/system/node_exporter.service << EOF
> [Unit]
Description=Node Exporter
After=network.target

[Service]
Type=simple
User=nobody
Group=nogroup
ExecStart=/usr/local/bin/node_exporter
Restart=always

[Install]
WantedBy=multi-user.target
EOF

[Unit]
Description=Node Exporter
After=network.target

[Service]
Type=simple
User=nobody
Group=nogroup
ExecStart=/usr/local/bin/node_exporter
Restart=always

[Install]
WantedBy=multi-user.target
ubuntu@ip-10-0-15-89:/tmp$ sudo systemctl daemon-reload
ubuntu@ip-10-0-15-89:/tmp$ sudo systemctl start node_exporter
ubuntu@ip-10-0-15-89:/tmp$ sudo systemctl enable node_exporter
ubuntu@ip-10-0-15-89:/tmp$ sudo systemctl status node_exporter
● node_exporter.service - Node Exporter
     Loaded: loaded (/etc/systemd/system/node_exporter.service; enabled; preset: enabled)
     Active: active (running) since Wed 2026-06-10 15:18:24 UTC; 54min ago
   Main PID: 17879 (node_exporter)
      Tasks: 5 (limit: 4520)
     Memory: 16.8M (peak: 18.3M)
        CPU: 95ms
     CGroup: /system.slice/node_exporter.service
             └─17879 /usr/local/bin/node_exporter

Jun 10 16:04:15 ip-10-0-15-89 node_exporter[17879]: time=2026-06-10T16:04:15.972Z level=ERROR source=http.go:231 msg="error encoding and sending metric family: write tcp [::1]:9100->[::1]:506>
Jun 10 16:04:15 ip-10-0-15-89 node_exporter[17879]: time=2026-06-10T16:04:15.972Z level=ERROR source=http.go:231 msg="error encoding and sending metric family: write tcp [::1]:9100->[::1]:506>
Jun 10 16:04:15 ip-10-0-15-89 node_exporter[17879]: time=2026-06-10T16:04:15.972Z level=ERROR source=http.go:231 msg="error encoding and sending metric family: write tcp [::1]:9100->[::1]:506>
Jun 10 16:04:15 ip-10-0-15-89 node_exporter[17879]: time=2026-06-10T16:04:15.972Z level=ERROR source=http.go:231 msg="error encoding and sending metric family: write tcp [::1]:9100->[::1]:506>
Jun 10 16:04:15 ip-10-0-15-89 node_exporter[17879]: time=2026-06-10T16:04:15.972Z level=ERROR source=http.go:231 msg="error encoding and sending metric family: write tcp [::1]:9100->[::1]:506>
Jun 10 16:04:15 ip-10-0-15-89 node_exporter[17879]: time=2026-06-10T16:04:15.972Z level=ERROR source=http.go:231 msg="error encoding and sending metric family: write tcp [::1]:9100->[::1]:506>
Jun 10 16:04:15 ip-10-0-15-89 node_exporter[17879]: time=2026-06-10T16:04:15.972Z level=ERROR source=http.go:231 msg="error encoding and sending metric family: write tcp [::1]:9100->[::1]:506>
Jun 10 16:04:15 ip-10-0-15-89 node_exporter[17879]: time=2026-06-10T16:04:15.972Z level=ERROR source=http.go:231 msg="error encoding and sending metric family: write tcp [::1]:9100->[::1]:506>
Jun 10 16:12:13 ip-10-0-15-89 systemd[1]: [🡕] /etc/systemd/system/node_exporter.service:8: Special user nobody configured, this is not safe!
Jun 10 16:12:30 ip-10-0-15-89 systemd[1]: [🡕] /etc/systemd/system/node_exporter.service:8: Special user nobody configured, this is not safe!

ubuntu@ip-10-0-15-89:/tmp$ curl http://localhost:9100/metrics | head -5
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0# HELP go_gc_duration_seconds A summary of the wall-time pause (stop-the-world) duration in garbage collection cycles.
# TYPE go_gc_duration_seconds summary
go_gc_duration_seconds{quantile="0"} 2.4852e-05
go_gc_duration_seconds{quantile="0.25"} 3.4299e-05
go_gc_duration_seconds{quantile="0.5"} 3.6631e-05
100  8192    0  8192    0     0   496k      0 --:--:-- --:--:-- --:--:--  500k
curl: (23) Failure writing output to destination
ubuntu@ip-10-0-15-89:/tmp$ docker exec prometheus wget -O- http://host.docker.internal:9100/metrics | head -5
wget: bad address 'host.docker.internal:9100'
ubuntu@ip-10-0-15-89:/tmp$ sudo nano /home/ubuntu/grafana-stack/prometheus.yml
ubuntu@ip-10-0-15-89:/tmp$ cd ~/grafana-stack
ubuntu@ip-10-0-15-89:~/grafana-stack$ docker compose restart prometheus
no such service: prometheus
ubuntu@ip-10-0-15-89:~/grafana-stack$ docker restart prometheus
prometheus
ubuntu@ip-10-0-15-89:~/grafana-stack$ curl http://localhost:9090/api/v1/targets | grep -A10 "node"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   584  100   584    0     0  94041      0 --:--:-- --:--:-- --:--:-- 97333
{"status":"success","data":{"activeTargets":[{"discoveredLabels":{"__address__":"node-exporter:9100","__metrics_path__":"/metrics","__scheme__":"http","__scrape_interval__":"1m","__scrape_timeout__":"10s","job":"node"},"labels":{"instance":"node-exporter:9100","job":"node"},"scrapePool":"node","scrapeUrl":"http://node-exporter:9100/metrics","globalUrl":"http://node-exporter:9100/metrics","lastError":"","lastScrape":"0001-01-01T00:00:00Z","lastScrapeDuration":0,"health":"unknown","scrapeInterval":"1m","scrapeTimeout":"10s"}],"droppedTargets":[],"droppedTargetCounts":{"node":0}}}
ubuntu@ip-10-0-15-89:~/grafana-stack$




