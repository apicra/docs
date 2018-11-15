# docs
Documentation | Apicra Docs

# What it's?
ApiCra works on Mac, Linux, Windows, and more. 
Access to Remote development environments force users to give up their software application. 
ApiCra works on your local system with the tools you're already familiar with. 


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

## Moudularisation, over public and private repositories
Installation of new packets should by possible over repositories url, to clone it and use it

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
        
### pobranie zmiennej z config do uzycia w pliku apicra.yaml

    {os.bash.config.extension}
    {os.bash.default.extension}
    
