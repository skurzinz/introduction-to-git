# Hi!

@ul
- Questions? Interrupt! 
- Language: Deutsch, slides in English
- This is very brief. 
    - Links to other introductions and full documentation available
@ulend

# Introduction

@ul
- Versioning is a concept known to Historians
- Git is a tool useful for 
    - collaborative versioning
    - attribution of changes
    - timeline
- changes are reversible
@ulend

# What about the name? 

@ul
- just a pronouncable 3-letter word 
- no collision with standard unix commands
- means "stupid person" (https://en.wiktionary.org/wiki/git)
@ulend

# What is git made for? 

@ul
- development / code
- (uncompressed) string-based data
@ulend

# What is it not made for? 

@ul
- binary data, e.g.
    - images
    - binary executables
    - zipped files such as .docx and other office file formats
- why not? 
    - hard to diff
@ulend

# Principal concepts of git

@ul
- working copy
- index
- remote repository
- local repository
- stash
- no "server/client" setup
@ulend

# How does git work in practice?

@ol
1. *clone* or create (*init*) a repository
2. make changes
3. *add* to index 
4. *commit* with a message documenting changes
5. *push* to remote
@olend

# How does git work in practice? (contd)

@ol
6. collaborators *pull* the changes
7. merge changes 
    - automatically if conflict-free
    - git tracks conflicts to be resolved manually
8. *commit* merges
9. *push* 
@olend

# Why would we care? 

@ul
- Messy states of e.g. change-tracking in standard word processors
- collaboration
    - attribution / responsibility
    - access control
- "short term 'backup'"
@ulend

# Question round

@ul
- ? 
@ulend

# Git branches

@ul
- standard: master
- n different states of the index
- Git stores differences between *commit*ted states
- a branch is a pointer to a specific state
@ulend

# Git flow branching

@ul
- master
- release
- development 
- feature 
- hotfix
@ulend

see https://m.infos.seibert-media.net/Productivity/Git-Workflows+-+Der+Gitflow-Workflow.html
# Git branches (contd)

@ol
1. a. git *branch* | git *checkout* -b branchname 
…  
5. if necessary on remotes:
    - *push* -u origin branchname  
    otherwise delete: 
    - git checkout development && git merge branchname && git branch -d branchname
@ulend

Branches are throwaway material

# Question round

@ul
- ? 
@ulend

# Installation

@ul
- Git SCM Download: https://git-scm.com/download
- GitHub Desktop: https://desktop.github.com/
@ulend

# Tools for Git 

@ul
- Git comes as a command line tool
- those who want to dig deeper: look into `./.git/`
- Graphical interfaces see https://git-scm.com/downloads, e.g.
    - SourceTree
    - GitAhead
    - GitHub Desktop
    - TortoiseGit
    - gitg 
- Some text/code editors/IDEs offer native/plugin Git support
- Web interfaces (covered in lesson02)
@ulend

# Use cases in the room

@ul
- this presentation: https://github.com/skurzinz/introduction-to-git.git
- https://github.com/KONDE-AT/maechtekongresse.git
- https://gitlab.com/acdh-oeaw/ministerratsprotokolle/
- https://github.com/travelogues
- https://github.com/qhod
@ulend


# Practical example

@ul
- register at https://github.com
- I'll allow you to directly add to the `introduction-to-git` repository
@ulend

# Exercise 1

@ul
- add any text file to the `text-files` folder 
- basic rendering is applied if you use  
    markdown syntax (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
@ulend

# Short break until 1530

