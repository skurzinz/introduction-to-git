# Git Version Control for Historians 

Vienna, Austria, 2020-06-22 

a very brief introduction.

2020-06-22, IHB, 1400-1730, Stephan Kurz

## Schedule | Overview

- 1400 Introduction 
- 1430 Installation 
- 1445 Hands-on (1) 
- 1515 Pause
- 1530 Git platforms (GitLab, GitHub)
- 1600 Hands-on (2) 
- 1645 End/open questions

<!-- lesson01 --> 

## Hi!

- Questions? Interrupt! 
- Language: Deutsch, slides in English
- This is very brief. 
    - Links to other introductions and full documentation available

## Introduction

- Versioning is a concept known to Historians
- Git is a tool useful for 
    - collaborative versioning
    - attribution of changes
    - timeline
- changes are reversible

## What about the name? 

- just a pronouncable 3-letter word 
- no collision with standard unix commands
- means "stupid person" (https://en.wiktionary.org/wiki/git)

## What is git made for? 

- development / code
- (uncompressed) string-based data

## What is it not made for? 

- binary data, e.g.
    - images
    - binary executables
    - zipped files such as .docx and other office file formats
- why not? 
    - hard to diff

## Principal concepts of git

- working copy
- index
- remote repository
- local repository
- stash
- no "server/client" setup

## How does git work in practice?

1. *clone* or create (*init*) a repository
2. make changes
3. *add* to index 
4. *commit* with a message documenting changes
5. *push* to remote

## How does git work in practice? (contd)

6. collaborators *pull* the changes
7. merge changes 
    - automatically if conflict-free
    - git tracks conflicts to be resolved manually
8. *commit* merges
9. *push* 

## Why would we care? 

- Messy states of e.g. change-tracking in standard word processors
- collaboration
    - attribution / responsibility
    - access control
- "short term 'backup'"

## Question round

- ? 

## Git branches

- standard: master/main 
- n different states of the index
- Git stores differences between *commit*ted states
- a branch is a pointer to a specific state

## Git flow branching

- master/main
- release
- development 
- feature 
- hotfix


see https://m.infos.seibert-media.net/Productivity/Git-Workflows+-+Der+Gitflow-Workflow.html

## Git branches (contd)

1. a. git *branch* | git *checkout* -b branchname 
2. make changes
3. *add* to index 
4. *commit* with a message documenting changes
5. if necessary on remotes:
    - *push* -u origin branchname  <br/>otherwise delete: 
    - git checkout development && git merge branchname && git branch -d branchname

Branches are throwaway material

## Question round

- ? 

## Installation

- Git SCM Download: https://git-scm.com/download
- GitHub Desktop: https://desktop.github.com/

## Tools for Git 

- Git comes as a command line tool
- Graphical interfaces see https://git-scm.com/downloads, e.g.
SourceTree, GitAhead, GitHub Desktop, TortoiseGit, gitg 
- Some text/code editors/IDEs offer native/plugin Git support
- Web interfaces (covered after the break)

## Use cases in the room

- this presentation: https://github.com/skurzinz/introduction-to-git.git
- https://github.com/KONDE-AT/maechtekongresse.git
- https://gitlab.com/acdh-oeaw/ministerratsprotokolle/
- https://github.com/travelogues
- https://github.com/qhod


## Practical example

- register at https://github.com
- I'll allow you to directly add to the `introduction-to-git` repository

## Exercise 1

- add any text file to the `text-files` folder 
- basic rendering is applied if you use <br/>markdown syntax (<https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>)

## Short break until 1600

<!-- lesson02 --> 

## GitHub: One web implementation

- https://github.com <br/>demo

## GitHub: One web implementation (contd)

- offers server for projects using Git
- concept of "fork" (branched copy)
- owned by Microsoft since 2019
- community features around Git
    - starring, watching
    - issue tracking
- user management
- private | public repositories
- build integration
- used internally at ACDH-CH / ÖAW (<https://github.com/acdh-oeaw/>)

## GitLab: Another web implementation

- https://gitlab.com <br/>demo

## GitLab: Another web implementation (contd)

- can be self-hosted
- user management
- "projects" group related repositories
- issue tracking
- Continuous Integration (CI) 
- GitHub *pull requests* are called *merge requests*
- only *Maintainer*+ level members can work on master
- used internally at ACDH-CH (<https://gitlab.oeaw.ac.at/>)

## Question round

- ? 

## Exercise 2

personalized tasks 

- create one private repo each to hold your respective edition TEI data 
- think about a folder/file structure together that should be followed in these repos

## Further reading

- https://rogerdudler.github.io/git-guide/index.de.html
- https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf
- https://education.github.com/git-cheat-sheet-education.pdf
- https://github.com/acdh-oeaw/tool-gallery-5.1.git
- https://github.com/acdh-oeaw/Teaching_CBS4DH/blob/master/lectures/git.md
- https://git-scm.com/book/en/v2


slides: https://gitpitch.com/skurzinz/introduction-to-git (not any longer)
