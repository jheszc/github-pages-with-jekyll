---
title: "Install NodeJS Debian"
date: 2021-02-10
---

Step 1: Update APT index
Run the apt update command on your Ubuntu / Debian Linux to update package repository contents database.

sudo apt update

Step 2: Install Node.js on Ubuntu / Debian Linux
Install Node.js 14 on Ubuntu / Debian by first installing the required repository.

curl -sL https://deb.nodesource.com/setup_14.x | sudo bash -

then

sudo apt -y install nodejs

Verify the version of Node.js installed.

$ node  -v

If you need Node Development tools, install them with the command:

sudo apt -y install gcc g++ make

To install the Yarn package manager, run:

curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update && sudo apt install yarn


