Useful commands for common git tasks.

### git commands

| Command    | Description                       |
| ---------- | --------------------------------- |
| `git init` | Initialize a local Git repository |

### gpg commands

| Command                                                             | Description                                 |
| ------------------------------------------------------------------- | ------------------------------------------- |
| `gpg --full-generate-key`                                           | Generate a gpg key (2.1.17 or greater)      |
| `gpg --list-secret-keys --keyid-format=long`                        | Prints both public and private gpg key id   |
| `gpg --armor --export <key-id>`                                     | Prints gpg public key in ASCII armor format |
| `gpg -a --export user@github.com > user-public-key.txt`             | Export gpg public key file                  |
| `gpg -a --export-secret-keys user@github.com > user-secret-key.asc` | Export gpg private key file                 |
| `gpg --export-ownertrust > user-ownertrust-db.txt`                  | Export gpg ownertrust db file               |
| `gpg --import user-secret-key.asc`                                  | Import gpg private key file                 |
| `gpg --import-ownertrust user-ownertrust-db.txt`                    | Import gpg ownertrust db file               |

---

### gpg issues

| Issues                                                     | Solution                                                 |
| ---------------------------------------------------------- | -------------------------------------------------------- |
| `gpg: can't connect to the agent: IPC connect call failed` | To fix this, re-import your private key & ownertrust db. |
