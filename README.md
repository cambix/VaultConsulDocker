
# VaultConsulDocker
corrected code for: http://pcarion.com/2017/04/30/A-consul-a-vault-and-a-docker-walk-into-a-bar..html

Vault Bash Completion:
```sh
sudo wget https://git.io/v1kgz -O /usr/local/etc/bash_completion.d/vault-bash-completion
```

To start up run the consul container first:
```sh
docker-compose -f consul.yml up
docker-compose -f vault.yml up
```
To stop containers
```sh
docker-compose -f consul.yml down
docker-compose -f vault.yml down
```

With AWS Secrets:
```sh
aws ecr get-login --no-include-email --region us-east-1
```
