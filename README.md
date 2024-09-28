+---------------------------+
|                           |
|       Quick-Git (qgit)    |
|                           |
+---------------------------+

Quick-Git (qgit) is a bash script that simplifies common Git operations. Currently, it combines the `git add`, `git commit`, and `git push` commands into a single, easy-to-use command: `qgit push`. This tool is designed to streamline your Git workflow and save you time.

## Installation

### Step 1: Clone the repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/qgit.git
cd qgit
```

### Step 2: Make the script executable

Run the following command to make the script executable:

```bash
chmod +x qgit
```

### Step 3: Add to PATH

#### Windows

1. Open the Start menu and search for "Environment Variables"
2. Click on "Edit the system environment variables"
3. Click the "Environment Variables" button
4. Under "System variables", find the "Path" variable and click "Edit"
5. Click "New" and add the full path to the directory containing the `qgit` script
6. Click "OK" on all windows to save the changes

Alternatively, you can use Git Bash on Windows and follow the Linux instructions.

#### Linux and Mac

1. Open your shell configuration file (`~/.bashrc`, `~/.zshrc`, or similar) in a text editor
2. Add the following line at the end of the file, replacing `/path/to/qgit` with the actual path:

   ```bash
   export PATH="/path/to/qgit:$PATH"
   ```

3. Save the file and run `source ~/.bashrc` (or your corresponding config file) to apply the changes

## Usage

To use qgit, simply run:

```bash
qgit push -a -m "Your commit message"
```

This will add all changes, commit with the specified message, and push to the remote repository.

To add specific files or use wildcards:

```bash
qgit push -f file1.py *.js -m "Your commit message"
```

This will add the specified files (in this example, `file1.py` and all `.js` files), commit with the message, and push to the remote repository.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the GPL3.0 License.
```
