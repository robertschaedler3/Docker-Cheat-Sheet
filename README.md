# Docker-Cheatsheet

## Articles
* [Dockerizing Angular CLI App](https://mherman.org/blog/dockerizing-an-angular-app/)

## Helpful Commands

Create a DigitalOcean Droplet with `docker-machine`:
```bash
docker-machine create \
  --driver digitalocean \ 
  --digitalocean-access-token <API ACCESS TOKEN> \
  <DROPLET NAME>
```

Connect `docker-machine` to an existing DigitalOcean Droplet:
```bash
docker-machine create \
  --driver generic \
  --generic-ip-address <DROPLET IPv4> \
  --generic-ssh-user root \
  --generic-ssh-key="~/.ssh/id_rsa" \
  <DROPLET NAME>
```
*Note: On Windows you may have to provide the full path to your ssh key*

