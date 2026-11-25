# Multi-User Document Editor

A C project for editing a shared document from multiple user processes. It includes terminal and browser interfaces.

## Requirements

Use Linux or WSL. On Ubuntu, install the compiler, Make, and ncurses:

```sh
sudo apt update
sudo apt install build-essential libncurses-dev
```

## Download and build

```sh
git clone https://github.com/ali-noor110/Multi_User-Document-Editor.git
cd Multi_User-Document-Editor
make
```

## Run in the terminal

Start the owner in one terminal:

```sh
./owner
```

Choose **3. Add user** in the menu. Then, in another terminal, start that user (replace `alice` with the username you added):

```sh
./user alice
```

Choose **10. Exit** in the owner menu when finished.

## Run in a browser

Instead of `./owner`, start the web server:

```sh
./web_server
```

Open [http://127.0.0.1:8765](http://127.0.0.1:8765) in your browser. Sign in as admin to manage users, or sign in with a username added by the admin.

Stop the server with `Ctrl+C`.

## Clean build files

```sh
make clean
```
