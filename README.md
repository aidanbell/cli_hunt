# CLI HUNT

## Finding Keys
As a newly hired SysAdmin, you need to clean up the file system of a team of developers. This team consists of 5 users: Alice, Doug, Nicole, Rebecca, and Tom (from MySpace). There's also a program that you're installing, called "AutoSysAdmin", which you'd really like to get up and running so you can play some video games at work. The only problem is, it needs all of the dev's Secret Key, which is stored somewhere in each user's folder.

All that you know about the system, is that there is a `usr` directory that contains each users data, and an `mnt` directory that has system related files inside. Each user has three directories: `dev` for all work related files, `docs` for documents, and `pics` for photos. From there, you don't know how each user has decided to organize their data.

```
.
├── README.md
├── mnt
│   ├── c
│   └── d
└── usr
    ├── ali
    │   ├── dev
    │   ├── docs
    │   └── pics
    ├── dug
    │   ├── dev
    │   ├── docs
    │   └── pics
    ├── nic
    │   ├── dev
    │   ├── docs
    │   └── pics
    ├── reb
    │   ├── dev
    │   ├── docs
    │   └── pics
    └── tom
        ├── dev
        ├── docs
        └── pics
```

The instructions for the installation are in the AutoSysAdmin folder, which is installed in Program_Files, either in the C drive or D drive (you can't remember). Those drives are located at `/mnt`. 

1. Find and read the instructions for AutoSysAdmin. It will be located in `Program_Files/AutoSysAdmin`, but the problem is there's a `Program_Files` in both `mnt/c` and `/mnt/d`, make sure you find the right one!
    > Commands you'll need:
    >
    > `cd`, `ls`, `cat`

2. Find each users secret key! There is a `log.txt` file somewhere in the `/mnt` directory, inside of a `boot` directory. That file will tell you the last project that each user was working on, which might be a good first place to check. 
    > Commands you'll need:
    > 
    >`cd`, `ls`, `cat`

    _HINT: use `cat` to read files quickly in your terminal. Things marked Important might lead you to your keys_

3. Once you find each key, make a copy of it! This would also be a good time to rename the file if you need to. 
    > Commands you'll need:
    >
    > `cp`

4. Move your newly copied key to where it's supposed to go!
    > Commands you'll need:
    >
    > `mv`

5. Finish up any left other instructions in the installation instructions. 


### BONUS:
Create a Symlink from the `AutoSysAdmin/usr/keys` directory to the `usr/asa/dev` directory. 