# trivial-twitter-v1

[![Project Status: Inactive – The project has reached a stable, usable state but is no longer being actively developed; support/maintenance will be provided as time allows.](https://www.repostatus.org/badges/latest/inactive.svg)](https://www.repostatus.org/#inactive)
[![Project License](https://img.shields.io/github/license/jordan396/trivial-twitter-v1.svg)](https://img.shields.io/github/license/jordan396/trivial-twitter-v1.svg)
[![Latest Commit](https://img.shields.io/github/last-commit/jordan396/trivial-twitter-v1/master.svg)](https://img.shields.io/github/last-commit/jordan396/trivial-twitter-v1/master.svg)
[![Repo Size](https://img.shields.io/github/repo-size/jordan396/trivial-twitter-v1.svg)](https://img.shields.io/github/repo-size/jordan396/trivial-twitter-v1.svg)
[![GitHub Followers](https://img.shields.io/github/followers/jordan396.svg?label=Follow)](https://img.shields.io/github/followers/jordan396.svg?label=Follow)

Simple socket application in C, with the following features:
  - Clients can upload *tweets* to and download *tweets* from a server. 
  - Upload/Download requests are secured using passphrases to prevent unauthorized requests.
  - Server stores only the latest *tweet* uploaded. 
  - *tweets* cannot exceed 150 characters.

![](./gifs/demo-v1.gif)

## Folder Structure
```
.
├── client         
│   ├── ttweetcli       // Executable for the client side
│   ├── ttweetcli.c     // Implementation file for the client side
│   └── ttweetcli.h     // Header file used for ttweetcli.c
├── README.md
├── gifs
│   └── demo-v1.gif     // The cool gif you see up there ^
└── server
    ├── ttweetser       // Executable for the client side
    ├── ttweetser.c     // Implementation file for the server side
    └── ttweetser.h     // Header file used for ttweetser.c
```
*Files are documented according to Doxygen*

## Installation
### Server
1. Clone this repository.

  `git clone https://github.com/Jordan396/trivial-twitter-v1.git`

2. Navigate to this directory. 

3. Execute executable on your preferred port.

  `server/ttweetser <ServerPort>`

### Client
1. Clone this repository.

  `git clone https://github.com/Jordan396/trivial-twitter-v1.git`

2. Navigate to this directory. 

3. To upload a tweet:

  `client/ttweetcli -u <ServerIP> <ServerPort> "message"`

4. To download a tweet:

  `client/ttweetcli -d <ServerIP> <ServerPort>`
