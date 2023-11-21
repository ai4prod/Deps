# Deps
Repository to handle ai4prod deps libraries


# How to Use

Ref https://docs.google.com/document/d/1IFR1F_PNsB0GA6Lv8FqiqXvEyYO1NNhyU3bEapt5ZME/edit#heading=h.2q0q4jkv5ngh

Each folder inside Bin/x86 and Bin/arm is a folder tracked with dvc. 

Now you have 3 remotes

windows
linux 
jetson 

each remote is paired with a remote folder on google drive

NOTE: We share deps as compressed file in order to reduce download time from remote server. 
Once download you need to unpach the file downloaded in the same folder.

This is useful because the deps folder are changed once in a while and we do not have frequent update
of this libraries
 

# How to push

## Windows
dcv add path/to/windows/windows_deps.rar
dvc push windows.dvc -r windows

this will push the change inside path/to/windows/ to remote folder tracked for windows remote

## Linux 
dcv add path/to/windows/linux_deps.rar
dvc push linux.dvc -r linux

## Jetson
dcv add path/to/jetson/jetson_deps.rar
dvc push jetson.dvc -r jetson


# How to pull
dvc pull  -r {remote name}

## example
dvc pull  -r jetson

