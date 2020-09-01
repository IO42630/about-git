###Git <br><br>

#### Areas 
* 1-3 are local.
* 1-4 may be called trees.
<br><br>

###### 1. Working Directory
* "physical" directory in which repo was initialized.
* contains files,
    * some of which are already *indexed* by git,
    * while others are not.
<br><br>

###### 2. Staging Area
* collection of all files that are indexed by git.
    * `add <file>` adds a file to index.
<br><br>

###### 3. Local Repository
* `commit` adds changes in indexed files to the local repo.
    * 1..n files can be committed in a single commit.
    * `HEAD` points to last commit.
        * i.e. commiting a change, moves the head to said change.
<br><br>

###### 4. Remote Repository
* 
* is created with `git init --bare`
    * this makes it impossible to commit
    * one can only push.
<br><br>

###### 5. Live Version 
<br><br><br><br>

####Transitions
| | |
---|---
`1 -> 2` | `add <file>`
`2 -> 3` | `commit`
`3 -> 4` | `push <origin> <branch>`
`3 <- 4` | `fetch`
`1 <- 3` | `merge`
`1 <- 4` | `pull`



#### Utility CMD
* `git status`