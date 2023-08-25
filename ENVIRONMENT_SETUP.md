# Environment Setup Guide

**Outline**:
- [Node Installations](#node-installations)
  - [NVM](#nvm)
  - [Node](#node)
  - [JSON-server](#json-server)
  - [Vite](#vite)
  - [express](#express)
  - [nodemon](#nodemon)
  - [pg](#pg)
- [VS Code Extensions](#vs-code-extensions)
  - [GitLens](#gitlens)
  - [Draw.io Integration](#drawio-integration)
  - [ESLint](#eslint)
  - [Prettier](#prettier)
  - [PostgreSQL](#postgresql-for-vs-code)
  - [Jest](#jest)
  - [Live Server](#live-server)
- [Applications/Software](#applicationssoftware)
  - [PostgreSQL](#postgresql-for-software)
  - [Postman](#postman)
  - [PuTTY on Windows](#putty-on-windows)
- [Configuring SSH keys for GitHub](#configuring-ssh-keys-for-github)

## Node Installations

### NVM

1. **macOS/Linux**:
    ```bash
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
    ```

   After installation, restart the terminal or run the following command to access `nvm`:

    ```bash
    export NVM_DIR="$HOME/.nvm"
    [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
    ```

2. **Windows**:
    - Download the installer from [here](https://github.com/coreybutler/nvm-windows/releases).
    - Follow the installation instructions.

3. Verify the installation:

    ```bash
    nvm --version
    ```

### Node

1. With `NVM` installed, you can install the latest stable version of node:

    ```bash
    nvm install node
    ```

2. Set the newly installed version as the default:

    ```bash
    nvm alias default node
    ```

3. Verify the Node and npm versions:

    ```bash
    node -v
    npm -v
    ```

### JSON-server

1. **macOS/Linux/Windows**:
    - Install JSON-server globally using npm:

    ```bash
    npm install -g json-server
    ```

2. Verify the installation:

    ```bash
    json-server --version
    ```

### Vite

1. **macOS/Linux/Windows**:
    - Install Vite globally using npm:

    ```bash
    npm install -g create-vite
    ```

2. Verify the installation:

    ```bash
    create-vite --version
    ```

### express

1. **macOS/Linux/Windows**:
    - Install Express generator globally using npm. This tool helps in scaffolding an Express application:

    ```bash
    npm install -g express-generator
    ```

2. Verify the installation:

    ```bash
    express --version
    ```

### nodemon

1. **macOS/Linux/Windows**:
    - Install nodemon globally using npm. Nodemon is a utility that monitors for changes in files and automatically restarts the node application:

    ```bash
    npm install -g nodemon
    ```

2. Verify the installation:

    ```bash
    nodemon --version
    ```

### pg

1. **macOS/Linux/Windows**:
    - Install `pg` (Node PostgreSQL client) globally using npm:

    ```bash
    npm install -g pg
    ```

2. No direct version verification command for `pg` when installed globally. However, once you incorporate it into a project, you can require and check its version.

Absolutely. For each VS Code extension, I will provide the general installation steps, a link to its official page on the VS Code marketplace, and any specific notes or requirements related to the extension.

---

## VS Code Extensions

### GitLens

1. **Installation**:
    - Open VS Code.
    - Go to Extensions view (`Ctrl+Shift+X`).
    - Search for `GitLens`.
    - Click on the Install button.

2. [**Official Marketplace Link**](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)

3. **Notes**:
    - GitLens supercharges the Git capabilities built into Visual Studio Code.
    - Requires Git to be installed.

### Draw.io Integration

1. **Installation**:
    - Open VS Code.
    - Go to Extensions view (`Ctrl+Shift+X`).
    - Search for `Draw.io Integration`.
    - Click on the Install button.

2. [**Official Marketplace Link**](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)

3. **Notes**:
    - This extension integrates Draw.io into VS Code.
    - Save diagrams as `.drawio`, `.drawio.png`, or `.drawio.svg`.

### ESLint

1. **Installation**:
    - Open VS Code.
    - Go to Extensions view (`Ctrl+Shift+X`).
    - Search for `ESLint`.
    - Click on the Install button.

2. [**Official Marketplace Link**](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

3. **Notes**:
    - Integrates ESLint JavaScript into VS Code.
    - For ESLint to work with your project, you should have the ESLint configuration set up either locally or globally.

### Prettier

1. **Installation**:
    - Open VS Code.
    - Go to Extensions view (`Ctrl+Shift+X`).
    - Search for `Prettier - Code formatter`.
    - Click on the Install button.

2. [**Official Marketplace Link**](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

3. **Notes**:
    - Prettier is an opinionated code formatter.
    - Supports many languages and integrates with most editors.
    - You might want to set Prettier as your default formatter in VS Code settings.

### PostgreSQL for VS Code

1. **Installation**:
    - Open VS Code.
    - Go to Extensions view (`Ctrl+Shift+X`).
    - Search for `PostgreSQL`.
    - Click on the Install button.

2. [**Official Marketplace Link**](https://marketplace.visualstudio.com/items?itemName=ms-ossdata.vscode-postgresql)

3. **Notes**:
    - Adds rich support for PostgreSQL to Visual Studio Code.
    - Useful features like connecting to PostgreSQL, running queries, and exploring databases.

### Jest

1. **Installation**:
    - Open VS Code.
    - Go to Extensions view (`Ctrl+Shift+X`).
    - Search for `Jest`.
    - Click on the Install button.

2. [**Official Marketplace Link**](https://marketplace.visualstudio.com/items?itemName=Orta.vscode-jest)

3. **Notes**:
    - Provides a rich jest runner for Visual Studio Code — great for practicing TDD and running unit tests in real-time.

### Live Server

1. **Installation**:
    - Open VS Code.
    - Go to Extensions view (`Ctrl+Shift+X`).
    - Search for `Live Server`.
    - Click on the Install button.

2. [**Official Marketplace Link**](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

3. **Notes**:
    - Launch a local development server with live reload feature for static and dynamic pages.

---

Remember to restart VS Code after installing extensions to ensure they're fully activated.

Certainly! I've incorporated a verification step for PostgreSQL on each platform. 

---

## Applications/Software

### PostgreSQL for Software

**PostgreSQL** is a powerful, open-source object-relational database system. Here are the installation methods and their pros and cons:

1. **macOS**:
   - **Postgres.app**:
     1. Download and install from [Postgres.app official site](https://postgresapp.com/).
     2. Move to Applications folder and start.
     - **Pros**: GUI tool, easy to use, includes many additional tools.
     - **Cons**: Specific to macOS.
     3. **Verification**:
        ```bash
        psql --version
        ```
   - **Homebrew**:
     1. If you don't have Homebrew, install it by following instructions [here](https://brew.sh/).
     2. Install PostgreSQL:
        ```bash
        brew install postgresql
        ```
     3. Start PostgreSQL:
        ```bash
        brew services start postgresql
        ```
     - **Pros**: Easy to manage and update.
     - **Cons**: Requires Homebrew.
     4. **Verification**: 
        ```bash
        psql --version
        ```

   - **Manual Installation**:
     - Download from the official [PostgreSQL site](https://www.postgresql.org/download/macosx/).
     - **Pros**: Complete control over configuration.
     - **Cons**: More manual steps; not as user-friendly.
     - **Verification**:
        ```bash
        psql --version
        ```

   - [Additional Resources for macOS](https://www.postgresql.org/download/macosx/)

2. **Windows**:
   - **pgAdmin/Interactive Installer**:
     1. Download from the official [PostgreSQL site](https://www.postgresql.org/download/windows/).
     2. Run the installer.
     - **Pros**: Provides pgAdmin, a popular PostgreSQL management tool.
     - **Cons**: Graphical installation might be less flexible for advanced users.
     3. **Verification**: Open Command Prompt and type:
        ```bash
        psql --version
        ```

   - **Windows Subsystem for Linux (WSL)**:
     - Allows running Linux distributions. PostgreSQL can be installed as on a regular Linux machine.
     - **Pros**: Closer to a Linux environment; allows running many Linux tools.
     - **Cons**: Requires setting up WSL.
     - **Verification**: In WSL terminal:
        ```bash
        psql --version
        ```

   - [Additional Resources for Windows](https://www.postgresql.org/download/windows/)

3. **Linux**:
   - **Package Manager** (for Ubuntu as an example):
     1. Update package lists:
        ```bash
        sudo apt update
        ```
     2. Install PostgreSQL:
        ```bash
        sudo apt install postgresql postgresql-contrib
        ```
     - **Pros**: Easy to manage and update.
     - **Cons**: Specific to Linux distributions. The commands vary between distros.
     3. **Verification**: 
        ```bash
        psql --version
        ```

   - **Source**:
     - Download and compile from source code.
     - **Pros**: Complete control over installation and configuration.
     - **Cons**: Requires more manual steps, dependencies.
     - **Verification**: 
        ```bash
        psql --version
        ```

   - [Additional Resources for Linux](https://www.postgresql.org/download/linux/)

### Postman

**Postman** is a popular tool for API testing.

1. **macOS/Windows/Linux**:
   - **Download and Install**:
     1. Go to the official [Postman Downloads page](https://www.postman.com/downloads/).
     2. Choose your OS and download the installer.
     3. Follow the installation prompts.

### PuTTY on Windows

**PuTTY** is an SSH and telnet client for Windows. It will be used when you connect to your AWS EC2 instance when you deploy your final project.

1. **Windows**:
   - **Download and Install**:
     1. Visit the official [PuTTY Download Page](https://www.putty.org/).
     2. Download the `.msi` file that matches your system (32-bit or 64-bit).
     3. Run the installer and follow the prompts.

   - **Notes**:
     - On macOS and Linux, SSH is typically available natively through the terminal, which is why PuTTY is especially relevant for Windows users.

---

## Configuring SSH Keys for GitHub

You need to do this if you try this command:

```bash
ssh -T git@github.com
```
and you get something that says 

```bash
git@github.com: Permission denied (public key).
```

if you run 

```bash
cat ~/.ssh/id_rsa.pub
```

If you don't see anything, then you can generate a new key with the following command. 
(Skip this step if you saw the key printed to the terminal already)

```bash
ssh-keygen -t rsa -b 4096 -C "your_github@email.com"
```

You'll get a few prompts here, you can confirm the default file location. If you don't
want to have to enter your credentials every time you push to GitHub, you can hit enter
twice more to leave the passphrase blank. Once the key has been generated, you can copy
it to the clipboard with the following command:

```
cat ~/.ssh/id_rsa.pub | pbcopy
```

Note, on Linux, you'll want to use something like `xclip` instead of pbcopy:

```
cat ~/.ssh/id_rsa.pub | xclip -sel clip
```

Or if you'd rather not install anything, you can just open the file and select all and copy:

```
code ~/.ssh/id_rsa.pub
```

Login to GitHub and go to [your ssh key settings](https://github.com/settings/keys)

### Click the Add SSH key button

In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal Mac, you might call this key "Personal MacBook Air".

### Paste in your SSH key

Your key should be in the clipboard from before. Next you can click the button.

### Click the Add SSH key button

You may be asked to confirm your password at this point.

### Fill in the confirm password form and submit

Finally, to test this out, you can run the following command again to test the SSH connection to GitHub:

```bash
ssh -T git@github.com
```

If all is well, you'll see something like this:

```
Hi DakotaLMartinez! You've successfully authenticated, but GitHub does not provide shell access.
```

And you're good to go! 👍