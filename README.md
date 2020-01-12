# :cloud: APicra documentation
Documentation | Apicra Docs

# What it's?
ApiCra works on Mac, Linux, Windows, and another systems. 
Access to Remote development environments force users to give up their software application. 
ApiCra works on your local system with the tools you're already familiar with. 

##  For what?
Apicra is open package system for bash files.
library based on .bat/.ssh files

## For Whom?
supports programmers in daily software development, in each area, where are necessary
bash scripts for automatisation.

Apicra is a set of tools used to define and execute scripts and services that automate software development, testing and delivery.
Supports and uses existing tools for DEVOPS

## History

### 2019.06 Devops flow tickets
+ help with daily git, npmjs usages
+ can sent in one time ticket, push, and publish project on npmjs, github
+ has internal variables
https://github.com/apicra/win-ticket-version-flow

### 2019.05, Devops packages designed for windows
https://github.com/apicra/npm-github-win

### 2018, Start with Devops - all in one
https://github.com/apicra/devops


## Modules

Apicra is opened for technologies.

## IDEAS
if You want to check your machine over apicra scripts:
https://serverscope.io/trials/740M#io

### Scripts over API with using apicra-ssh
https://github.com/apicra/ssh

Should be possible to execute on any server:
memory
size
cpu

## Moudularisation over environment
Installation of new packets should by possible over repositories url, to clone it and use it
for all, public and private repositories, most popular git solutions such: 
+ github
+ bitbucket
+ gitlab

## How to startr project with apicra
### 1. Go to your project path

### 2. Download script:
apicra-install.sh / apicra-install.bat 
and execute

    sh apicra-install.sh
or 

    ./apicra-install.bat


### 3. Initialisation, generate the config file: apicra.yaml

    apicra init
    
### 4. start using in console, with menu
  
    apicra
    

## Struktura:

### Pliki: skrypty, stale, zmienne srodowiskowe
  ukladane w odniesieniu do systemu
  
  
### Zmienne w zaleznosci od systemu

+ os
  + win
    + bash
      config.yaml / default.yaml
        extension = sh
        
