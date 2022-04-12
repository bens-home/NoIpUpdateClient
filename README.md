# NoIpUpdateClient
This is a docker-compose setup to use the `coppit/no-ip` docker image that will automatically update my domains with No-Ip

[coppit/no-ip](https://hub.docker.com/r/coppit/no-ip) has over 5 million downloads so that's why I am just using that instead of writing my own. The [No-ip dynamic update client](https://www.noip.com/download) requires an interactive setup, so setting that data via enviornment variables is the easiest way to go.

## Get Started

## Enviornment Setup

We need to tell the no-ip client about our username, password, and what domain we want to update. We can do this with a config file that no-ip2 will read when it starts. Copy or rename the `config/noip.conf.template` file to be just `config/noip.conf`. This is what no-ip2 will read to get your username and password.

## Start the container

To start the container run:

```
docker-compose up -d
```

To check the status, run:

```
docker-compose logs
```