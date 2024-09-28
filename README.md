```
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

To use qgit, you have several options:

1. Add all changes, commit, and push to the current branch:

```bash
qgit push -a -m "Your commit message"
```

2. Add specific files or use wildcards, commit, and push to the current branch:

```bash
qgit push -f file1.py *.js -m "Your commit message"
```

3. Add all changes, commit, and push to a specific branch:

```bash
qgit push -a -o branch_name -m "Your commit message"
```

4. Add specific files, commit, and push to a specific branch:

```bash
qgit push -f file1.py *.js -o branch_name -m "Your commit message"
```

Flags:
- `-a`: Add all changes (equivalent to `git add .`)
- `-f`: Specify files to add (can use wildcards)
- `-m`: Provide the commit message (required)
- `-o`: Specify the branch to push to (optional)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
```