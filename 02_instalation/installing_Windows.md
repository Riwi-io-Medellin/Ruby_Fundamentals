### Installing Ruby on Windows Using RubyInstaller

On Windows, RubyInstaller is the easiest and most popular way to install Ruby. It provides a precompiled version of Ruby along with a Development Kit (MSYS2), which is essential for building gems that require native extensions.

---

### Step 1: Download RubyInstaller

1. Visit the official [RubyInstaller website](https://rubyinstaller.org/).
2. Download the **Ruby+Devkit** version for the latest Ruby release (recommended).

---

### Step 2: Run the RubyInstaller Executable

1. Locate the downloaded installer (`rubyinstaller-<version>.exe`) and double-click it to start the installation.
2. Follow the installation wizard:
   - **Choose Installation Directory**: Leave the default directory (`C:\Ruby<version>`) or specify a custom directory.
   - **Check Options**: Ensure that "Add Ruby executables to your PATH" is checked.

---

### Step 3: Install MSYS2 and Development Tools

1. Once the Ruby installation completes, a window will prompt you to install MSYS2 (Development Kit). Click **Yes** to continue.
2. Follow the instructions to install MSYS2, which provides essential tools for compiling Ruby gems.

---

### Step 4: Verify Ruby Installation

1. Open a new Command Prompt or PowerShell window.
2. Check the Ruby version by running:
   ```bash
   ruby -v
   ```
   You should see the installed Ruby version.

---

### Step 5: Install Bundler (Optional but Recommended)

Bundler is a tool for managing Ruby gem dependencies. Install it by running:

```bash
gem install bundler
```

---

### Step 6: Install Additional Ruby Gems

With Ruby installed, you can install additional gems using the `gem` command. For example:

```bash
gem install rails
```

---

### Step 7: Update RubyInstaller and MSYS2 (Optional)

To keep your Ruby environment up-to-date:
1. Open the `Start Command Prompt with Ruby` (installed during the RubyInstaller setup).
2. Run the following command to update MSYS2:
   ```bash
   ridk install
   ```

---

### Managing Multiple Ruby Versions on Windows

If you need to manage multiple Ruby versions on Windows, you can use tools like **uru** or **pik**. These tools allow you to install multiple versions of Ruby and switch between them.

1. **Install Uru**:
   - Download the latest Uru binary from its [GitHub page](https://bitbucket.org/jonforums/uru/wiki/Home).
   - Follow the instructions to set up Uru for version management.

---

### Troubleshooting

1. **Command Not Found**: If Ruby commands like `ruby` or `gem` are not recognized, ensure that Ruby is correctly added to your system PATH. You can manually add the Ruby installation path (e.g., `C:\Ruby<version>\bin`) to the PATH environment variable.
2. **MSYS2 Issues**: If MSYS2 fails to install or update, you can manually update it by running:
   ```bash
   ridk install
   ```
3. **Gems Not Installing**: Some gems require native extensions to be built. Ensure MSYS2 is installed and up-to-date.

---

### Additional Tips

- Use **PowerShell** or **Windows Terminal** for a better command-line experience on Windows.
- Explore the RubyInstaller DevKit for building native extensions and compiling gems.

---

With RubyInstaller, you can quickly set up a Ruby development environment on Windows, making it easy to start coding and exploring the language.


Once you have Ruby installed in your environment, you can execute any script with a `.rb` extension by using the `ruby` command followed by the name of your script file. For example:

```bash
ruby test.rb
```

### [Back to menu](../README.md)