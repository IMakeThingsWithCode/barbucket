# barbucket
A utility for catching thoughts before they skitter away

I commonly find myself thinking of clever and nonsenical one-liners and I wanted a way to store them, so I decided to make a program that could be opened quickly whenever I got one of these thoughts. I want to keep it simple and adaptable, and just dump all thoughts into a text file.

## Dependencies
- bash
- zenity
- xsel

## Setup
Installing dependencies:
```shell
sudo apt update
sudo apt install zenity xsel
```

Cloning the repo:
```shell
mkdir -p ~/.barbucket/.app/
cd ~/.barbucket/.app/
git clone https://github.com/IMakeThingsWithCode/barbucket.git
chmod +x ./barbucket/shortcut ./barbucket/shortcut
```

If you use these commands for setup, it will install both apps to `~/.barbucket/.app/barbucket/`.
By default, collections will be located at `~/.barbucket/`, and you can open the collections at any time with a standard file viewer or text editor.

Running:
- Application (viewer) run `~/.barbucket/.app/barbucket/barbucket`
- Shortcut (quick add) run `~/.barbucket/.app/barbucket/shortcut`

## You should bind the `shortcut` script to a key!
Obviously the purpose of this app is mostly defeated if you have to open a terminal and run the app through it every time, so it's recommended to use your shortcut management app of choice to bind a key combo to run `~/.barbucket/.app/barbucket/shortcut`.

## Usage
This repo contains two seperate apps. The main one is `shortcut`, and the other one (`barbucket`) is just a viewer. `barbucket` can be used, but you could also just use a text editor.
### shortcut (quick add)
1. Run tool
2. Write a thought
3. Select a collection to save the thought to
### barbucket (collection viewer)
1. Save thoughts with other tool
2. Run this tool
3. Select a collection
4. View thoughts in selected collection
5. Copy one of the thoughts or exit

## Todo
- [x] First prototype
    - [x] Can be keybound
    - [x] Prompts for thought
    - [x] Dumps thought to text file
- [x] GUI update
    - [x] Pick save location, like pinterest
        - [x] Divide into boards, one file per
- [x] Thought viewer for boards
    - [x] Select board
    - [x] Thought actions
        - [x] View
        - [x] Copy
- [x] Write setup guide
    - [ ] Test on another device / fresh install