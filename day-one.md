## 🚀 System Initialization

### Setup and System Prep

* Boot each G3 and verify hardware is working.
* Recover Windows 11 Key before OS wipe using this command: (save to usb or write it down) 

```powershell
  (Get-WmiObject -query 'select * from SoftwareLicensingService').OA3xOriginalProductKey
```

- [ ] Download Ubuntu / Mint ISO or USB file to install from.
- [ ] Use [Rufus](https://rufus.ie/en/) to create bootable USB
- [ ] Install Ubuntu / Linux Mint
- [ ] System Customization
  - [ ] Wallpaper
  - [ ] Window Color
  - [ ] Terminal Selection / Setup
    - [ ] [Ghostty](https://ghostty.org/) or [Warp](https://on.warp.dev/home)
    - [ ] Install `zsh` and change it to your default shell with `chsh -s $(which zsh)`
    - [ ] Install [oh my zsh](https://ohmyz.sh/)
    - [ ] Install & Setup [Starship](https://starship.rs/) or [Powerlevel10k](https://github.com/romkatv/powerlevel10k)
- [ ] Install `nvim`, `curl`, `neofetch`, `figlet`, `lolcat`, and `btop`
- [ ] Setup folders - you’ll store your projects here, day by day. Think of each folder as a memory sector in your code disk.

```bash
mkdir -p ~/derezzed/day-one
mkdir -p ~/derezzed/day-two
mkdir -p ~/derezzed/day-three
```

## 🧪 The Grid

### Terminal Basics

* List files `ls`, `ls -al`, `ls -lh`
* Change directories `cd`, `cd ..`, `cd ~/Downloads`
* Make directories `mkdir derezzed`, `mkdir -p path/to/grid`
* Create files `touch`, `nvim`, `cat`
* Remove files `rm file`, `rm -r folder/`
* Rename files `mv filename filename2`
* Move files `mv filename ../filename`
* Forbidden cmd `rm -rf /` (explain why this is dangerous)
* Search `find`, `grep`, `locate`, `which`
* History `history`, `Ctrl + R`, 
* Pipe Operator
  * `ls | wc -l` - Count how many files in a directory
  * `ps aux | head -n 5` - Show top 5 running processes
  * `ls -l | grep ".sh"` - Filter for whatever's in the quotes
  * The pipe character takes output from the left and PIPES it into the command on the right
 
Complete the following tasks to continue: 
- [ ] Navigate to your Downloads folder using `cd`
- [ ] Create a folder named `my-lightcycle` and verify it exists using `ls`
- [ ] Use `touch` to create a file called `users.txt` then delete it
- [ ] Use `find` to locate `nvim` on your system
- [ ] Count the number of `.sh` files in your home directory using pipes

### 📜 Basic Bash Script

* Create our first bash script
  * Create a new file inside your `day-one` directory called `init-light-cycles.sh` using `touch`
  * Open the file using `nvim` and paste in the following code:

```bash
#!/bin/bash
mkdir -p ~/derezzed/day-one/lightcycles
cd ~/derezzed/day-one/lightcycles
touch lightcycle-white.txt lightcycle-blue.txt lightcycle-yellow.txt lightcycle-red.txt 
echo "Scanning directory contents..."
ls -alh ~/derezzed/day-one/lightcycles
```

What this does:
1. Tells the computer this is a bash script using the she bang syntax `#!/bin/bash`
2. Creates a directory
3. Creates some files in the directory
4. Outputs some text to the terminal
5. Lists the files

### 🔐 Who Are You?

Complete the following tasks to continue:
- [ ] Create a new file called `verify.sh` with the following contents. 
- [ ] Make the file executable with `chmod +x [filename]`
- [ ] Run the file with `./[filename]`
- [ ] What is the output? Explain what you think this is doing.

```bash
#!/bin/bash
echo "What's your username?"
read USERNAME
if [ "$USERNAME" == "tron" ]; then
  echo "Access granted, welcome to The Grid"
else
  echo "Access denied, Unknown Program, derezzed initiated!"
fi
```

### 🧑‍💻 On Your Own

- [ ] Create a basic script `initialize-grid.sh` in your `day-one` folder.
- [ ] Line `1` should have she bang `#!/bin/bash`
- [ ] Line `2` `echo` the following statement to the terminal `"Initializing The Grid..."`
- [ ] Line `3` use `figlet` to send `"TRON ONLINE"` via PIPE to `lolcat`
- [ ] Line `4` run `neofetch`
- [ ] Make the file executable with `chmod +x [filename]`
- [ ] Run the file with `./[filename]`


### Leveling Up

## Git, GitHub, VSCode

- [ ] Install git  `sudo apt install git`
- [ ] Install GitHub CLI `sudo apt install gh`
- [ ] Install VSCode
  - [ ] Install extensions `python`, `markdown preview`, `theme(s)`

### Create GitHub Profile

- [ ] Create a repo named exactly `github_username` on [GitHub.com](https://www.github.com)
- [ ] Clone locally via `cd ~/derezzed`, `gh repo clone username/username`, `cd username`
- [ ] Open this in vscode `code .`
- [ ] Add name, intro, fun emoji or ASCII art, GitHub stats badges, and a goal for Derezzed

## 🧰 Other Things to Check Out

* `systemd-analyze` - how long does it take your system to load and what part takes the longest
* `blame` - see exactly what slows down your system
