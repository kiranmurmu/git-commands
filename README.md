Useful commands for common git tasks.

### git commands

| Command                                               | Description                                  |
| ----------------------------------------------------- | -------------------------------------------- |
| `git init`                                            | initialize local repository                  |
| `git config user.name`                                | get local user name                          |
| `git config user.email`                               | get local user email                         |
| `git config --global user.name`                       | get global user name                         |
| `git config --global user.email`                      | get global user email                        |
| `git config user.name "<user_name>"`                  | set local user name                          |
| `git config user.email "<user_email>"`                | set local user email                         |
| `git config --global user.name "<user_name>"`         | set global user name                         |
| `git config --global user.email "<user_email>"`       | set global user email                        |
| `git add .`                                           | add all files not staged                     |
| `git add <file_name>`                                 | stage specific file                          |
| `git add <directory_name>`                            | stage entire directory                       |
| `git commit -m "<message>"`                           | commit changes                               |
| `git commit -s -m "<message>"`                        | sign and commit changes                      |
| `git status`                                          | check repository status                      |
| `git status -s`                                       | show brief repository status                 |
| `git branch -a`                                       | show all remote or local branches            |
| `git branch <branch_name>`                            | create new branch                            |
| `git branch -d <branch_name>`                         | delete branch                                |
| `git branch -m <branch_name> <new_branch_name>`       | rename a local branch                        |
| `git checkout <branch_name>`                          | checkout existing branch                     |
| `git checkout -b <new_branch_name>`                   | checkout and create new branch               |
| `git log`                                             | show changes                                 |
| `git log --oneline`                                   | show brief changes                           |
| `git log --summary`                                   | show detailed changes                        |
| `git merge <source_branch_name>`                      | merge changes into current branch            |
| `git merge <source_branch_name> <target_branch_name>` | merge source and target branche              |
| `git remote -v`                                       | show named remote repositories               |
| `git remote add origin <remote_repository_url>`       | add empty remote repository                  |
| `git clone <remote_repository_url>`                   | clone and add remote repository              |
| `git pull origin <branch_name>`                       | pull changes from specific remote branch     |
| `git pull`                                            | pull changes from remote repository          |
| `git push origin <branch_name>`                       | push branch to remote branch                 |
| `git push -u origin <branch_name>`                    | push changes to remote branch and remember   |
| `git push origin --delete <branch_name>`              | delete branch from remote repository         |
| `git push`                                            | push changes to remembered remote branch     |
| `git push —all`                                       | push all local branches to remote repository |

### gpg commands

| Command                                                          | Description                             |
| ---------------------------------------------------------------- | --------------------------------------- |
| `gpg --full-generate-key`                                        | generate gpg key (2.1.17 or greater)    |
| `gpg --list-secret-keys --keyid-format=long`                     | prints both public and private key id   |
| `gpg --armor --export <key_id>`                                  | prints public key in ascii armor format |
| `gpg -a --export <user_email> > user-public-key.txt`             | export public key file                  |
| `gpg -a --export-secret-keys <user_email> > user-secret-key.asc` | export private key file                 |
| `gpg --export-ownertrust > user-ownertrust-db.txt`               | export ownertrust db file               |
| `gpg --import user-secret-key.asc`                               | import private key file                 |
| `gpg --import-ownertrust user-ownertrust-db.txt`                 | import ownertrust db file               |
