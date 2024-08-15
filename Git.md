## [Return/Back to Course list.](Courses)
# Core Concepts
## Repository
* This is the storage location of your project.
* Local Repository -- Your personal copy of the project on your machine.
* Remote Repository -- A version of your project hosted on a server.
## Commit
* This is a snapshot of your project. It includes a message describing the changes.
## Branch
* This is a parallel version of your project. The main branch is usually called main or master. These allow you to work on new features without affecting the main project.
## Merge
* Merging combines changes from different branches into one. If you work on a new feature and want to add it to the main project, you merge it into the 'main' branch.
## Clone
* Cloning a Repository means creating a copy of the remote Repository on your Local machine.
## Pull
* Pulling means fetching changes from the remote Repository to your Local Repositoryand integrating them.
## Push
* Pushing means sending your local commits to the remote Repository.
## Staging Area
* The staging area is where you can prepare changes before commiting them. You add files to the staging area, then commit them to the Repository.
## Workflow
- git add <file>
- git commit -m "Commit message"
- git log
- git branch <branch-name> -- Create a branch named <branch-name>.
- git checkout <branch-name> -- Switch to branch named <branch-name>.
- Merge a branch:
  - git checkout main
  - git merge <branch-name>
- Clone a repository:
  - git clone <repository-url>
- Push Changes to Remote Repository:
  - git push <remote-repo-name> <branch-name>
- Pull Changes from Remote Repository:
  - git pull
# Advanced Git Features
## Branch Management:
  * Rename a Branch:
    * git branch -m <old-branch-name> <new-branch-name>
  * Delete a Branch:
    * git branch -d <branch-name>
  * View All Branches:
    * git branch
## Rebasing:
  - Rebasing is an alternative to merging. It moves or combines a sequence of commits to a new base commit.
  * Rebase a branch:
    - git checkout <feature-branch>
    - git rebase main
  - Rebasing rewrites commit history, which can make it cleaner, but be careful as it can lead to conflicts.
## Stashing:
  - Stashing lets you save changes that you aren't ready to commit yet.
  * Stash Changes:
    - git stash
  * Apply Stashed Changes:
    - git stash apply
  * View Stashes:
    - git stash list
## Undoing Changes:
  * Revert a Commit:
    - git revert <commit-id>
  * Reset to a Previous Commit:
    - git reset --hard <commit-id>
  * Remove Files from Staging:
    - git reset <file>
  * Remove Changes in Working Dir:
    - git checkout -- <file>
## Git Tags:
  - Tags are useful for marking specific points in history as important.
  * Create a Tag:
    - git tag -a v1.0 -m "Version 1.0"
  * Push Tags to Remote:
    - git push <remote-repo-name> --tags

