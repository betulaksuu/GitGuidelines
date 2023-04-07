# Separate Your Branches into Two Groups

### Main Branches

#### Master:

The origin/master branch represents the main branch of your application. The source code of HEAD is always in a production-ready state.

#### Develop:

The origin/develop branch is a branch that is parallel to the master branch. It stores the latest ready-for-release development changes. The source code of HEAD reflects the changes for the next release.

### Supporting Branches

#### Feature:
Feature branches are used to develop a feature for a future release. This branch exists as long as the feature is being developed, but eventually, it ends up being merged in the develop branch.

-   May branch off from: **develop**
-   May be merged into: **develop**
-   Branch naming convention: feature/name-of-feature (e.g feature/login)

**Example:**

    $ git checkout develop // Switched to branch develop
    $ git pull origin develop // get all up to date changes from develop
    $ git checkout -b feature/feature-name // Switched to new branch ‘feature/feature-name’
    $ git merge feature/name-of-feature // After it’s done it’s merged into the develop branch  (on branch develop)


#### Hotfix:

Hotfix branches are used for when a critical bug is found in production and a fix is needed immediately. When a critical bug in production arises a hotfix branch is created so that the problem is resolved within the appropriate time frame.

 - May branch off from: **master**
 - May be merged into: **master or develop**
 - Branch naming convention:  **hotfix/description-of-fix**  (e.g  **hotfix/login-fix**)

**Example:**

    $ git checkout master // Switched to branch master
    $ git pull origin master // get all up to date changes from master
    $ git checkout -b hotfix/description-of-fix // Switched to new branch ‘hotfix/description-of-fix’
    $ git merge hotfix/description-of-fix // After it’s done it’s merged into the develop branch (on branch master)

#### Bugfix:

Bugfix branches are used for when a bug is found that has not been deployed on production yet. Probably found during the QA process, a bug that is not of critical importance is found and for the purposes of solving it a bugfix branch is created.

 - May branch off from:  **develop**
 - May be merged into:  **develop**
 - Branch naming convention:  **bugfix/description-of-bug**  (e.g  **bugfix/admin-login-bug**)

**Example:**

    $ git checkout develop // Switched to branch develop
    $ git pull origin develop // get all up to date changes from develop
    $ git checkout -b bugfix/description-of-bug // Switched to new branch ‘bugfix/description-of-bug’
    $ git merge bugfix/description-of-bug // After it’s done it’s merged into the develop branch (on branch develop)
