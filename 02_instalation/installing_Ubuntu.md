### Installing Ruby on Ubuntu Using RVM (Ruby Version Manager)

RVM (Ruby Version Manager) is a popular tool for managing multiple Ruby versions on your system. It simplifies the installation process and allows you to switch between different Ruby versions effortlessly. Here's the updated step-by-step guide for installing Ruby on Ubuntu using RVM.
"Alternatively, you can follow RVM's official documentation for a detailed, step-by-step guide. Visit https://rvm.io/ to get started."

---

### Step 1: Update System Packages

Before installing RVM, update your system packages to ensure you have the latest versions.

```bash
sudo apt update && sudo apt upgrade -y
```

---

### Step 2: Install Required Dependencies

Install the dependencies needed for RVM and Ruby installation.

```bash
sudo apt install -y curl gpg build-essential libssl-dev libreadline-dev zlib1g-dev
```

---

### Step 3: Install GPG Keys for RVM

RVM requires GPG keys for verification. Import the keys by running:

```bash
gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
```

For an additional key (in case the primary key has issues):

```bash
gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
```

---

### Step 4: Install RVM

Run the following command to install RVM along with the latest stable Ruby version:

```bash
\curl -sSL https://get.rvm.io | bash -s stable
```

Once the installation is complete, load RVM into your shell session:

```bash
source ~/.rvm/scripts/rvm
```

---

### Step 5: Verify RVM Installation

Check if RVM is installed correctly:

```bash
rvm --version
```

If the version is displayed, RVM is installed successfully.

---

### Step 6: Install Ruby

With RVM installed, you can now install the latest stable Ruby version:

```bash
rvm install ruby --default
```

This will download and install the latest Ruby version and set it as the default version.

---

### Step 7: Verify Ruby Installation

Check the installed Ruby version:

```bash
ruby -v
```

You should see the latest Ruby version displayed.

---

### Step 8: Install Bundler (Optional but Recommended)

Bundler is a gem manager for Ruby that helps manage dependencies. Install it using:

```bash
gem install bundler
```

---

### Step 9: Managing Multiple Ruby Versions (Optional)

If you need to use multiple Ruby versions, you can install other versions and switch between them using RVM. For example:

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

### Step 10: Update RVM (Optional)

To ensure you have the latest version of RVM, you can update it by running:

```bash
rvm get stable
```

---

### Troubleshooting

- If you encounter permission issues, ensure your user has proper access to the `~/.rvm` directory.
- Add RVM to your shell startup file to load it automatically:
  ```bash
  echo 'source ~/.rvm/scripts/rvm' >> ~/.bashrc
  source ~/.bashrc
  ```

---

By following these steps, you will have Ruby installed on your Ubuntu system using RVM, allowing you to manage and switch between multiple Ruby versions effortlessly.


Once you have Ruby installed in your environment, you can execute any script with a `.rb` extension by using the `ruby` command followed by the name of your script file. For example:

```bash
ruby test.rb
```

### [Back to menu](../README.md)