# BetterMarzban-scripts
Scripts for BetterMarzban

> If this repository is private, set the `MARZBAN_GITHUB_TOKEN` (or `GITHUB_TOKEN`) environment variable before running the installer, or be ready to paste a GitHub token with `repo` access when prompted.

Docker images are published to GitHub Container Registry as `ghcr.io/arman2122/bettermarzban`.  
Use `--version vX.Y.Z` to pin a release tag that was built by the CI workflow.

## Installing Marzban
- **Install Marzban with SQLite**:

```bash
sudo bash -c "$(curl -sL https://github.com/Arman2122/BetterMarzban-scripts/raw/main/marzban.sh)" @ install
```

- **Install Marzban with MySQL**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/Arman2122/BetterMarzban-scripts/raw/main/marzban.sh)" @ install --database mysql
  ```

- **Install Marzban with MariaDB**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/Arman2122/BetterMarzban-scripts/raw/main/marzban.sh)" @ install --database mariadb
  ```
  
- **Install Marzban with MariaDB and Dev branch**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/Arman2122/BetterMarzban-scripts/raw/main/marzban.sh)" @ install --database mariadb --dev
  ```

- **Install Marzban with MariaDB and Manual version**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/Arman2122/BetterMarzban-scripts/raw/main/marzban.sh)" @ install --database mariadb --version v0.5.2
  ```

- **Update or Change Xray-core Version**:

  ```bash
  sudo marzban core-update
  ```


## Installing Marzban-node
Install Marzban-node on your server using this command
```bash
sudo bash -c "$(curl -sL https://github.com/Arman2122/BetterMarzban-scripts/raw/main/marzban-node.sh)" @ install
```
Install Marzban-node on your server using this command with custom name:
```bash
sudo bash -c "$(curl -sL https://github.com/Arman2122/BetterMarzban-scripts/raw/main/marzban-node.sh)" @ install --name marzban-node2
```
Or you can only install this script (marzban-node command) on your server by using this command
```bash
sudo bash -c "$(curl -sL https://github.com/Arman2122/BetterMarzban-scripts/raw/main/marzban-node.sh)" @ install-script
```

Use `help` to view all commands:
```marzban-node help```

- **Update or Change Xray-core Version**:

  ```bash
  sudo marzban-node core-update
  ```
