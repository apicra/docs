# :cloud: APicra documentation
Documentation | Apicra Docs

##  For what?
Apicra is open package system for bash files.
library based on .bat/.ssh files
Apicra is a set of tools used to define and execute scripts and services that automate software development, testing and delivery.
Supports and uses existing tools for DEVOPS
Apicra can have access to Remote development environments force users to give up their software application. 

## For Whom?
supports programmers in daily software development, in each area, where are necessary
bash scripts for automatisation.

# Where it Works?
ApiCra works on Mac, Linux, Windows, and another systems. 
ApiCra works on your local system with the tools you're already familiar with. 

## History

#### 2019.06 Devops flow tickets
https://github.com/apicra/win-ticket-version-flow
+ help with daily git, npmjs usages
+ can sent in one time ticket, push, and publish project on npmjs, github
+ has internal variables

| command | local files | remote github | remote NPMJS | shortcut to APICRA
| --- | --- | --- | --- | --- |
| -create.bat | create | create | --- | .apicra\\-project-create.bat %GIT_USER% %PROJECT% |
| -publish.bat | --- | push, tag | create | --- |
| **-ticket.bat** | --- | **push** | --- | --- |
| **-version.bat** | --- | **tag** | **update** | --- |
| -delete.bat | delete | delete | delete | .apicra\\-project-delete.bat %GIT_USER% %PROJECT%  |


#### 2019.05, Devops packages designed for windows
https://github.com/apicra/npm-github-win

#### 2018, Start with Devops - all in one
https://github.com/apicra/devops


## Modules

Apicra is opened for libraries, packages
now it is possbile to wirte new direkt on project

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
        
