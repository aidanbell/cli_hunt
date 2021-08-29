# AUTOSYSADMIN

## Getting Started

All you need to do, is make sure that each user has a file inside of `usr/keys` that contains their key. The name of the file must be their three character username, with the extension `.json`. For example, if you had a user named George, with a username `geo`, their file would be called `geo.json`.

## Setup

Once you have all of the keys in the folder, it's necessary to add a user directory for AutoSysAdmin. It will need to go with the rest of the user folders, must be called `asa`, and it needs to follow this structure:
```
asa
├── dev
│   └── start
│       └── startup.txt
└── dump
    └── log.txt
```