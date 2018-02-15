# Stellar to GraphQL

Medium Article:
https://medium.com/@tyvdh/building-stellar-apps-36303d0e6f45

Video Tutorials:
https://www.youtube.com/watch?v=qO1GhY3UeR8
https://www.youtube.com/watch?v=FdcTz3B-PH4
https://www.youtube.com/watch?v=8AnjmzTgry0

## "Quick" Start

```bash
## Install Docker
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
apt-get update
apt-cache policy docker-ce
apt-get install -y docker-ce
systemctl status docker

## Install Docker Compose
curl -L https://github.com/docker/compose/releases/download/1.19.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose

## Install glysh-docker repo
git clone https://github.com/TinyAnvil/glysh-docker.git
cd glysh-docker

## Run
docker-compose up
```

<!--
mechanic add api-test --host=api-test.gly.sh --backends=3001 --https=true --redirect-to-https=true
mechanic add core-test --host=core-test.gly.sh --backends=4001 --https=true --redirect-to-https=true
mechanic add horizon-test --host=horizon-test.gly.sh --backends=5001 --https=true --redirect-to-https=true

mechanic add api --host=api.gly.sh --backends=3000 --https=true --redirect-to-https=true
mechanic add core --host=core.gly.sh --backends=4000 --https=true --redirect-to-https=true
mechanic add horizon --host=horizon.gly.sh --backends=5000 --https=true --redirect-to-https=true
-->
