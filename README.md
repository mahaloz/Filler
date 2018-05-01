# Filler
Testing framework for determining the effectiveness of adversarial code on Driller (AFL + SE).
All tests were produced on Ubuntu 16.04 through the shellphish/mechaphish docker image.

## About

Considering the high rate of automation in binary analysis and exploitation, the question spawns: what methods do have to preventing automated hacking. The [Cyber Grand Challenge](https://www.darpa.mil/program/cyber-grand-challenge) (CGC) hosted by DARPA, proved that we are on the brink of automation, but an effective method to halting executors may be Adversarial code injects. 

## Purpose

The purpose of these test are to evaluate the *effectiveness* of Adversarial code injects on Symbolic Execution and Fuzzing.

## Test Components
* [About](README.md)
* [Test Design](Test-Design.md)
* [Replicating Test](Replicating-Test.md)
* [Results](Results.md)
* Misc Scripts
* [Future Research](Future-Research.md)

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
