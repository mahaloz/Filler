# Replicating the Test
The technical breakdown for running and testing binaries. Shellphuzz was used for Driller, and patcherex for patching

## Installing Driller, Patcherex, and Shellphish-QEMU
The simplest way to use Shellphish's Driller & Patcherex is through their mechaphish docker container

```bash
#insall docker
sudo apt-get install docker-ce

#pull the mechaphish container
sudo docker pull shellphish/mechaphish

#run the image with loaded binaries
sudo docker run -it --rm -v $PWD:/home/angr/Filler/ shellphish/mechaphish
```
## Running the initial binaries
Running the initial binaries is as simplea as invoking the shellphish-qemu cgc base with each binary. For example, running CADET_00001 once in the mechaphish docker:

```bash
~/.virtualenvs/angr-pypy/site-packages/shellphish_qemu/bin/shellphish-qemu-cgc-base ~/Filler/binaries_unpatched/CADET_00001
```



