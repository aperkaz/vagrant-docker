# vagrant-docker
[Vagrant](https://www.vagrantup.com/) Linux image, ready to rock deployments.

## Goal
Provide a portable, replicable and reliable working environment for professional and personal container development.

## Features
The base image is provisioned as follows:

### Base image
- [X] [14.04 64-bit Ubuntu](https://app.vagrantup.com/phusion/boxes/ubuntu-14.04-amd64)

## Management
### Box Management Commands
- Spin up the virtual environment (Vagrant-box). The environment is also provisioned:
```
vagrant up
```
- Provision the currently running environment (using `provision.sh` script):
```
vagrant box list
```
- Stop a running environment:
```
vagrant suspend
```
- Completely remove the environment:
```
vagrant destroy
```
### Miscellaneous
- Switch between between multiple terminals without GUI:
```
Alt + F1-F12
```
- Set the keyboard layout to Spanish (session):
```
setxkbmap -layout es
```
- Set the keyboard layout to Spanish (permanently). Reboot after:
```
apt-get install console-common
localectl set-x11-keymap es
localectl set-keymap es
```
## License
MIT © [Alain Perkaz](https://aperkaz.github.io)