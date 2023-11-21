# Deps
Repository to handle ai4prod deps libraries


# How to Use

Each folder inside Bin/x86 and Bin/arm is a folder tracked with dvc. 

Now you have 3 remotes

windows
linux 
jetson 

each remote is paired with a remote folder on google drive

# How to push

## Windows
dcv add path/to/windows
dvc push windows.dvc -r windows
## Linux 

dvc push linux.dvc -r linux

## Jetson
dvc push jetson.dvc -r jetson


# How to pull
dvc pull  -r {remote name}

## example
dvc pull  -r jetson

