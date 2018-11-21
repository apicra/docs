# :cloud: APicra documentation
Documentation | Apicra Docs

# What it's?
ApiCra works on Mac, Linux, Windows, and more. 
Access to Remote development environments force users to give up their software application. 
ApiCra works on your local system with the tools you're already familiar with. 

##  Do czego sluzy?
Apicra wspiera programiste w codziennym wytwarzaniu kodu.
Apicra to zestaw narzedzi sluzacych do definiowania i wykonywania skryptow i uslug automatyzujacych wytwarzanie, testowanie i dostarczanie oprogramowania.
Wspiera istniejace narzedzia dla DEVOPS


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
    

## Example config for apicra:
[apicra](apicra.yaml)
    
    
    


    to jest truktura danych i skryptow
    jeden moze wywolywac drugi
    moga sie zapetlac

    simple apicra:
      version: 1.1.0
      install:
      - {ssh.local} {project.path} {cmd.mysql.restore_from_test}
      - {ssh.test} {project.path} {cmd.mysql.backup}
      - {ssh.live} {project.path} {cmd.mysql.backup}

      xampp:    
        path: "c:/xampp"      
        ssh:
          type: 'docker_name'
          credentials:
        db:
          type: 'mysql'
          credentials: "keepass.file"
          backup: {ssh.local} \ {xampp.path} \ backup.bat
          restore: {ssh.local} \ {local.path} \ restore.bat

      docker:
        path: 
          html: "c:/"      
        ssh:
          type: 'docker_name'
          credentials:
        db:
          type: 'mysql'
          credentials: "keepass.file"
          backup: {ssh.local} {local.path} backup.sh
          restore: {ssh.local} {local.path} backup.sh
            - 
      test:
        path: "/"
        ssh: 'ssh credentials'
      live:
        path: "var/www"
        ssh: 'ssh credentials'
      backup:
        path: "var/www"
        ssh: 'ssh credentials'
