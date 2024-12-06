### Installing Ruby on macOS Using RVM (Ruby Version Manager)

RVM (Ruby Version Manager) is a powerful tool for managing multiple Ruby versions on macOS. It simplifies the installation process and allows you to easily switch between different Ruby versions. Follow these updated steps to install Ruby on macOS using RVM.

---

### Step 1: Update macOS and Install Xcode Command Line Tools

Ensure your macOS is up-to-date and install Xcode Command Line Tools, which are required for compiling Ruby.

1. Update macOS:
   ```bash
   softwareupdate --install --all
   ```

2. Install Xcode Command Line Tools:
   ```bash
   xcode-select --install
   ```

---

### Step 2: Install Homebrew (if not already installed)

Homebrew is a package manager for macOS that simplifies the installation of dependencies.

1. Install Homebrew by running:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. Add Homebrew to your PATH (if not done automatically):
   ```bash
   echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zshrc
   eval "$(/opt/homebrew/bin/brew shellenv)"
   ```

3. Verify Homebrew installation:
   ```bash
   brew --version
   ```

---

### Step 3: Install Required Dependencies

Use Homebrew to install the dependencies needed for RVM and Ruby installation:

```bash
brew install gpg curl gnupg
```

---

### Step 4: Install GPG Keys for RVM

RVM requires GPG keys for verification. Import the keys by running:

```bash
gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
```

For an additional key (in case the primary key has issues):

```bash
gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
```

---

### Step 5: Install RVM

Run the following command to install RVM along with the latest stable Ruby version:

```bash
\curl -sSL https://get.rvm.io | bash -s stable
```

After installation, load RVM into your shell session:

```bash
source ~/.rvm/scripts/rvm
```

---

### Step 6: Verify RVM Installation

Ensure RVM is installed correctly by checking its version:

```bash
rvm --version
```

If the version is displayed, RVM has been installed successfully.

---

### Step 7: Install Ruby

With RVM installed, install the latest stable Ruby version:

```bash
rvm install ruby --default
```

This will download and install the latest Ruby version and set it as the default version.

---

### Step 8: Verify Ruby Installation

Check the installed Ruby version:

```bash
ruby -v
```

You should see the latest Ruby version displayed.

---

### Step 9: Install Bundler (Optional but Recommended)

Bundler is a gem manager that helps manage dependencies for your Ruby projects. Install it using:

```bash
gem install bundler
```

---

### Step 10: Managing Multiple Ruby Versions (Optional)

If you need to use multiple Ruby versions, RVM makes it easy to install and switch between them. For example:

1. Install another Ruby version:
   ```bash
   rvm install 3.1.4
   ```

2. Switch to a specific Ruby version:
   ```bash
   rvm use 3.1.4
   ```

3. Set a default Ruby version:
   ```bash
   rvm --default use 3.1.4
   ```

---

### Step 11: Update RVM (Optional)

To ensure you are using the latest version of RVM, update it with the following command:

```bash
rvm get stable
```

---

### Troubleshooting

- **RVM Not Loading Automatically**: Add RVM to your shell configuration file (e.g., `~/.zshrc` or `~/.bashrc`):
  ```bash
  echo 'source ~/.rvm/scripts/rvm' >> ~/.zshrc
  source ~/.zshrc
  ```

- **Permission Issues**: Ensure your user has the proper permissions to use RVM and Ruby by running:
  ```bash
  rvm group add rvm
  ```

---

By following these steps, you’ll have Ruby installed on your macOS system using RVM, enabling you to manage and switch between multiple Ruby versions seamlessly.

Once you have Ruby installed in your environment, you can execute any script with a `.rb` extension by using the `ruby` command followed by the name of your script file. For example:

```bash
ruby test.rb
```