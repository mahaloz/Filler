# Filler
Testing framework for determining the effectiveness of adversarial code on Driller (AFL + SE)
The test was produced on Ubuntu 16.04

## Installing Driller & Patcherex
The simplest way to use Shellphish's Driller & Patcherex is through their mechaphish docker container

```bash
#insall docker
sudo apt-get install docker-ce

#pull the mechaphish container
sudo docker pull shellphish/mechaphish

#run the image with loaded binaries
sudo docker run -it --rm -v $PWD:/home/angr/Filler/ shellphish/mechaphish
```

## Usage
