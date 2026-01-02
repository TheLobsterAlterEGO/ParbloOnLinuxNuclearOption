
# (arch) Linux and graphic tablet monitor setup (Parblo coast 16)

Consider this guide more like "nuclear option" when dealing with tablet moniotors from Parblo



## Reason

Due to lack of drivers for linux it is impossible to use tablet monitors from Parblo which is annoying since I'm an artist. 

## Why you shouldn`t use it

- It is a lazy solution 

- It requires a lot of resources to function properly (i gave up for my vm 12gb of ram memory and 8 vCPU allocations)

- Maybe you are a lucky person who has found drivers for their tablet drivers 


## Solutions you might want to consider before going on with this guide

 - [Drivers for Coast 22](https://github.com/dsevy/parblo-coast/tree/master)
 - [Drivers for Coast 10](https://github.com/Skrylar/parblo-coast)
 

## Core idea 

Basically my solution is straight forward 

    1. Setup Qemu/Kvm
    2. Run tiny11 iso on a vm
    3. Pass a usb from tablet to the vm
    4. Install drivers on to the vm
    5. Install program for drawing on to the same vm 
    6. Turn on fullscreen mode for vm and drag it on to second monitor which will be tablet



## Qemu/KvmSetup

there are a lot of guides how to do this 

[youtube video on how to do it fast](https://youtu.be/cN_a7NgBWX8?si=g94yoNq1Yi2GZ8Y6) 
    

## Tin11 iso (any windows iso is going to be fine)

I have chosen smallest iso thats why i went with tiny11

https://archive.org/download/tiny11_25H2


## Passing usb to the vm

- Go to hardware details of the windows vm 

- "Add hardware"

- "Usb host device" 

- Select your tablets usb

- (optional) set Startup Policy to optional

## Installing drivers 

- Go to parblo site 

- Download windows drivers for the tablet

- Install drivers 

## Install drawing app of your choosing

i hope i dont have to explain how to install it

## How to use!?!?!??

- Open vm in fullscreen on the tablet monitor 

- From there it should be same expirience as drawing on windows

## ISUES 

- [fixed] it does not support bidirectionall file drag and drop [Solution](https://github.com/silvercreeper356/virtiofs-guide?tab=readme-ov-file)
