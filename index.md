---
layout: default
---
`sudoankit$ man UNIXRoutine` :

[UNIX Routine](https://github.com/sudoankit/UNIXRoutine) is a **beautiful**, **minimal**, **essential** one page `UNIX` commands cheat sheet with geeky gif screenshots!

## The daily coffee. 
---

### `ls` : list all the files in the **current** directory. Dark Secrets.

À la carte :

- `ls -l` : long format, displaying Unix file types, permissions, number of hard links, owner, group, size, last-modified date and filename.

- `ls -f` : do not sort.

- `ls -a` : lists **hidden** files.

- `ls -F` : appends a character revealing the nature of a file. 

- `ls -R` : recursively lists subdirectories.

>Learn more about `ls` [here.](https://en.wikipedia.org/wiki/Ls)

Geeky Gif : 

![ls.gif](geekygifs/ls.gif)

---

### `cd` : change from anywhere to home directory. Welcome back, hon.

À la carte : 

- `cd ..` : go back one level.

- `cd ~username` : puts you in username's home directory. [UNIX ONLY]

- `cd ` : puts you in the user main directory. Home, folks.

- `cd some_fun_directory` : puts you in `some_fun_directory`. 

> if you are in `/usr`, typing `cd lol` will put you in `/usr/lol`, while `cd /lol` puts you in `/lol`.

Geeky gif :

![cd.gif](geekygifs/cd.gif)

---
 
### `rm` : removes references to objects from the filesystem.

In layman terms, it **removes a file** from the present directory.

À la carte : 

- `rm -r` : removes directories, removing the contents recursively beforehand.

- `rm -i` : interative removal of a file. Asks beforehand if you wanna die :)

- `rm -f` : may the **force** be with you. Forcefully removes the file without any confirmation prompts. 

- `rm -rf` : forcefully and recursively removes every single precious file.

> rm -rf , rm -rf /, rm -rf *, is frequently used in jokes and anecdotes about Unix disasters. **NEVER RUN THIS IN SUPERUSER UNLESS YOU KNOW WHAT YOU ARE DOING**.
Have a nice day.

---

### `apt-get` : Package manager for debian systems. 50% off this winters.

In layman terms, it's a package manager to install, delete, update, upgrade softwares directly from **command line** . 

À la carte : 

- `apt-get update` : Updates the list of packages you can install from various sources.

- `apt-get install package_name` : Downloads and install that package from the internet. Usually follows the above command.

- `apt-get purge package_name` : Completely removes the package. 

- `apt-get install -f package_name` : Download and install, and correct broken dependecies. Like if package A is dependent on package B to run, but package B is broken it may try to reinstall it.

- `apt-get autoremove` : removes unused packages automatically.

> All of these commands are generally preceded by sudo (super user do) which in noob speak translates to administrater privileges. The GUI app to do this effectively can be downloaded using `apt-get install synaptic` 

### `dnf` : Package manager. The next gen YUM with more YUMmy.

DNF or Dandified Yum is the next generation version of the Yellowdog Updater, Modified (yum), a package manager for RPM-based distributions(like Fedora).

À la carte : 

- `dnf update` : Updates the installed packages in your system.

- `dnf install package_name` : Searches the RPM repository for the package, downloads and installs it on the system.

- `dnf remove package_name` : Kicks out the specified package and flushes out all its files.

> Before running the above commands, you have to either get sudo access by entering `su` and then your password or by preceding the command with `sudo`.
 
---
Copyright [sudoankit.](https://github.com/sudoankit)
Licensed under the [MIT License.](https://raw.githubusercontent.com/sudoankit/UNIXRoutine/master/LICENSE)

<a href="https://github.com/sudoankit/UNIXRoutine" class="github-corner"><svg width="80" height="80" viewBox="0 0 250 250" style="fill:#151513; color:#fff; position: absolute; top: 0; border: 0; right: 0;"><path d="M0,0 L115,115 L130,115 L142,142 L250,250 L250,0 Z"></path><path d="M128.3,109.0 C113.8,99.7 119.0,89.6 119.0,89.6 C122.0,82.7 120.5,78.6 120.5,78.6 C119.2,72.0 123.4,76.3 123.4,76.3 C127.3,80.9 125.5,87.3 125.5,87.3 C122.9,97.6 130.6,101.9 134.4,103.2" fill="currentColor" style="transform-origin: 130px 106px;" class="octo-arm"></path><path d="M115.0,115.0 C114.9,115.1 118.7,116.5 119.8,115.4 L133.7,101.6 C136.9,99.2 139.9,98.4 142.2,98.6 C133.8,88.0 127.5,74.4 143.8,58.0 C148.5,53.4 154.0,51.2 159.7,51.0 C160.3,49.4 163.2,43.6 171.4,40.1 C171.4,40.1 176.1,42.5 178.8,56.2 C183.1,58.6 187.2,61.8 190.9,65.4 C194.5,69.0 197.7,73.2 200.1,77.6 C213.8,80.2 216.3,84.9 216.3,84.9 C212.7,93.1 206.9,96.0 205.4,96.6 C205.1,102.4 203.0,107.8 198.3,112.5 C181.9,128.9 168.3,122.5 157.7,114.1 C157.9,116.9 156.7,120.9 152.7,124.9 L141.0,136.5 C139.8,137.7 141.6,141.9 141.8,141.8 Z" fill="currentColor" class="octo-body"></path></svg></a><style>.github-corner:hover .octo-arm{animation:octocat-wave 560ms ease-in-out}@keyframes octocat-wave{0%,100%{transform:rotate(0)}20%,60%{transform:rotate(-25deg)}40%,80%{transform:rotate(10deg)}}@media (max-width:500px){.github-corner:hover .octo-arm{animation:none}.github-corner .octo-arm{animation:octocat-wave 560ms ease-in-out}}</style>
