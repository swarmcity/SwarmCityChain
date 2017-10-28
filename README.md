![Swarm City](https://github.com/swarmcity/sc-boardwalk-production/blob/master/images/icons/icon-48x48.png?raw=true "Swarm City")


# Swarm City
### SwarmCityChain

## Install dependencies

- git

   Install [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) commandline tool.

- docker

   Install [docker](https://docs.docker.com/engine/installation). The community edition (docker-ce) will work. In Linux make sure you grant permissions to the current user to use docker by adding current user to docker group, `sudo usermod -aG docker $USER`. Once you update the users group, exit from the current terminal and open a new one to make effect.

- docker-compose

   Install [docker-compose](https://docs.docker.com/compose/install)
   
**Note**:- Make sure you can run `git`, `docker ps`, `docker-compose` without any issue and without sudo command.

## Install SwarmCityChain

```
git clone https://github.com/swarmcity/SwarmCityChain.git
```

### Initialize 

```
cd SwarmCityChain
docker-compose up -d
````

### Configuration

#### Parity

Parity configuration file

`
conf/config.toml
`

More info about setting up parity:

[wiki](https://github.com/paritytech/parity/wiki/Configuring-Parity)

[parity-config-generator](https://paritytech.github.io/parity-config-generator/)

#### Docker-compose

Pesistent data stored on `./data`. 
* keys
* parity_chain
* parity_basepath