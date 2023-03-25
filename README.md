# iwe

an integrated writing environment for academic writing and research on the command line

## about

this is a repository for a bunch of dotfiles and scripts that constitute my "integrated writing environment".

at the heart of the environment is `vim`. i've been using vim for almost 10 years now, and am now incapable of using any other text editor. 

for my writing workflow, I cannot live without an auto-complete function for
citations. being able to type `@Le` and then hit Ctr-x-o to have a list of
bibtex cite-keys staring with `Le` appear saves minutes of searching, cutting,
and pasting. this functionality is provided by the `vim-pandoc` plugin for vim.

on the topic of bibliographies, since I am currently on a mac, I use `bibdesk` to manage my `.bib` files. `bibdesk` has a wonderful 'import from clipboard' function which saves a lot of time when adding citations. while I still manage my bibliographies manually, without using online tools, I feel that this strikes the right balance between control and ease of use.

i do all of my writing using markdown as a markup language for plain text files. i use `pandoc` for conversion to other formats, in particular to `.pdf`. for most projects, I write a `makefile` so that I can just run `make` to generate the output files. 

i use `git` to version control my files. i hardly use any of git's functionality, however. it is good to know that if I need to, I can find something somewhere in my commit history and revert and recover if need be. this is certainly better than saving multiple files with timestamps in the filenames as i used to. 

recently, i've been working on scripts using `fzf` and `rga` to improve how I search for files and the content of files on my computers. i now have far too many `.pdf` books to manually search for references. i am also far too lazy to add identifying information to the articles i download. i have tried to write scripts to help with this.

finally, since my work is split between my laptop and a desktop in the office, this environment needs to work on both machines. my plan is to manage this by setting variables on each machine that the scripts assume are available. unfortunately, I'm restricted to using `onedrive` at work for cloud storage. i treat my onedrive folder as something of a default root, with all of my other folders contained within it. so most of the variables are just paths to directories in my onedrive directory.

here are the command line tools that are essential to the setup, in something like order of importance:

* `vim` --- text editor
* `pandoc` --- document converter
* `make` --- tool to manage compilation and recompilation of output files
* `fzf` --- fuzzy finder 
* `rga` --- a faster grep for searching in files of various kinds
* `zsh` --- a shell

