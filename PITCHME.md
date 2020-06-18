---?color=linear-gradient(to right, #4286f4, ##fffff) @title[Git Version Control for historians]

@snap[west text-25 text-bold text-black] 
Git Version Control for Historians 
@snapend

@snap[south-west byline text-white text-06] Vienna, Austria, 2020-06-22 @snapend

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Welcome]

@snap[north h3-white span-100]
### Git Version Control for Historians 
@snapend

@snap[south span-100]
a very brief introduction.

2020-06-22, IHB, 1400-1730, Stephan Kurz
@snapend


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Schedule | Overview]

@snap[north h3-white]
#### Schedule | Overview
@snapend

- 1400 Introduction 
- 1430 Installation 
- 1445 Hands-on (1) 
- 1515 Pause
- 1530 Git platforms (GitLab, GitHub)
- 1600 Hands-on (2) 
- 1645 End/open questions


<!-- lesson01 --> 

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Hi!]

@snap[north h3-white]
#### Hi!
@snapend


- Questions? Interrupt! 
- Language: Deutsch, slides in English
- This is very brief. 
    - Links to other introductions and full documentation available


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Introduction]

@snap[north h3-white]
#### Introduction
@snapend


- Versioning is a concept known to Historians
- Git is a tool useful for 
    - collaborative versioning
    - attribution of changes
    - timeline
- changes are reversible


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[What about the name?]

@snap[north h3-white]
#### What about the name? 
@snapend


- just a pronouncable 3-letter word 
- no collision with standard unix commands
- means "stupid person" (https://en.wiktionary.org/wiki/git)


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[What is git made for?]

@snap[north h3-white]
#### What is git made for? 
@snapend


- development / code
- (uncompressed) string-based data


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[What is it not made for?]

@snap[north h3-white]
#### What is it not made for? 
@snapend


- binary data, e.g.
    - images
    - binary executables
    - zipped files such as .docx and other office file formats
- why not? 
    - hard to diff


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Principal concepts of git]

@snap[north h3-white]
#### Principal concepts of git
@snapend


- working copy
- index
- remote repository
- local repository
- stash
- no "server/client" setup


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Git in practice 1]

@snap[north h3-white]
#### How does git work in practice?
@snapend

@ol[](false)
1. *clone* or create (*init*) a repository
2. make changes
3. *add* to index 
4. *commit* with a message documenting changes
5. *push* to remote
@olend

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Git in practice 2]

@snap[north h3-white]
#### How does git work in practice? (contd)
@snapend

@ol[](false)
6. collaborators *pull* the changes
7. merge changes 
    - automatically if conflict-free
    - git tracks conflicts to be resolved manually
8. *commit* merges
9. *push* 
@olend

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Why?]

@snap[north h3-white]
#### Why would we care? 
@snapend


- Messy states of e.g. change-tracking in standard word processors
- collaboration
    - attribution / responsibility
    - access control
- "short term 'backup'"


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Questions?]

@snap[north h3-white]
#### Question round
@snapend


- ? 


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Git branches]

@snap[north h3-white]
#### Git branches
@snapend


- standard: master
- n different states of the index
- Git stores differences between *commit*ted states
- a branch is a pointer to a specific state


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Git flow branching]

@snap[north h3-white]
#### Git flow branching
@snapend


- master
- release
- development 
- feature 
- hotfix


see https://m.infos.seibert-media.net/Productivity/Git-Workflows+-+Der+Gitflow-Workflow.html
+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Git branches]

@snap[north h3-white]
#### Git branches (contd)
@snapend

@ol[](false)
1. a. git *branch* | git *checkout* -b branchname 
2. make changes
3. *add* to index 
4. *commit* with a message documenting changes
5. if necessary on remotes:
    - *push* -u origin branchname  <br/>otherwise delete: 
    - git checkout development && git merge branchname && git branch -d branchname
@olend

@snap[south span-100]
Branches are throwaway material
@snapend

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Questions?]

@snap[north h3-white]
#### Question round
@snapend


- ? 


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Installing git]

@snap[north h3-white]
#### Installation
@snapend


- Git SCM Download: https://git-scm.com/download
- GitHub Desktop: https://desktop.github.com/


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Tools for Git]

@snap[north h3-white]
#### Tools for Git 
@snapend


- Git comes as a command line tool
<!-- - those who want to dig deeper: look into `./.git/` -->
- Graphical interfaces see https://git-scm.com/downloads, e.g.
SourceTree, GitAhead, GitHub Desktop, TortoiseGit, gitg 
- Some text/code editors/IDEs offer native/plugin Git support
- Web interfaces (covered after the break)


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Use cases in the room]

@snap[north h3-white]
#### Use cases in the room
@snapend


- this presentation: https://github.com/skurzinz/introduction-to-git.git
- https://github.com/KONDE-AT/maechtekongresse.git
- https://gitlab.com/acdh-oeaw/ministerratsprotokolle/
- https://github.com/travelogues
- https://github.com/qhod



+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Practical example]

@snap[north h3-white]
#### Practical example
@snapend


- register at https://github.com
- I'll allow you to directly add to the `introduction-to-git` repository


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Exercise 1]

@snap[north h3-white]
#### Exercise 1
@snapend


- add any text file to the `text-files` folder 
- basic rendering is applied if you use <br/>markdown syntax (<https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>)


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[—— Break ——]

@snap[north h3-white]
#### Short break until 1530
@snapend



<!-- lesson02 --> 


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[GitHub: One web implementation]

@snap[north h3-white]
#### GitHub: One web implementation
@snapend


- https://github.com <br/>demo


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[GitHub: One web implementation]


@snap[north h3-white]
#### GitHub: One web implementation (contd)
@snapend


- offers server for projects using Git
- concept of "fork" (branched copy)
- owned by Microsoft since 2019
- community features around Git
    - starring, watching
    - issue tracking
- user management
- private | public repositories
- build integration
- used internally at ACDH-CH


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[GitLab: Another web implementation]


@snap[north h3-white]
#### GitLab: Another web implementation
@snapend


- https://gitlab.com <br/>demo


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[GitLab: Another web implementation]


@snap[north h3-white]
#### GitLab: Another web implementation (contd)
@snapend


- can be self-hosted
- user management
- "projects" group related repositories
- issue tracking
- Continuous Integration (CI) 
- GitHub *pull requests* are called *merge requests*
- only *Maintainer*+ level members can work on master
- used internally at ACDH-CH


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Questions?]


@snap[north h3-white]
#### Question round
@snapend


- ? 


+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Exercise 2]


@snap[north h3-white]
#### Exercise 2
@snapend

personalized tasks 

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Exercise 2 MRP]

@snap[north h3-white]
#### Exercise 2 MRP
@snapend


- create a branch of the `mp-data` repo for your respective volume and propose a change in GitLab via a Merge Request
<!-- - Travelogues -->
<!--    - fork the github pages repo and fix a typo using a GitHub pull request -->

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Exercise 2 maechtekongresse]

@snap[north h3-white]
#### Exercise 2 maechtekongresse
@snapend


- change your remote to https://github.com/KONDE-AT/maechtekongresse.git
- pro action: create a GitLab account and create a kongress-docker repo and a dockerfile in there to get the CI to deploy the GitHub app+data repo

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Exercise 2 QHOD]

@snap[north h3-white]
#### Exercise 2 QHOD
@snapend



- create one private repo each to hold your respective edition TEI data 
- think about a folder/file structure together that should be followed in these repos

+++?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[Further reading]


@snap[north h3-white]
#### Further reading
@snapend


- https://rogerdudler.github.io/git-guide/index.de.html
- https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf
- https://education.github.com/git-cheat-sheet-education.pdf
- https://github.com/acdh-oeaw/tool-gallery-5.1.git
- https://github.com/acdh-oeaw/Teaching_CBS4DH/blob/master/lectures/git.md
- https://git-scm.com/book/en/v2







---?color=linear-gradient(180deg, #5289F7 18%, white 18%)
@title[That's it!]

@snap[north h3-white]
Thanks!
@snapend

slides: 

https://gitpitch.com/skurzinz/introduction-to-git
