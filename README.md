# browserrun
A small script making it quick and easy to debug JavaScript files using your default browser's developer tools using a single command.

## Install
###Clone the directory (fx. to a directory containing your scripts or git folders)
`git clone https://github.com/SimonDein/browserrun.git ~/myGitDirectory/browserrun`

Optional: Symlink the file to an appropriate destination (fx. where you keep your local commdand scripts)
`ln -s ~/myGitDirectory/browserrun/browserrun ~/myScripts`

###Add executable to path
add to `~/.bash_profile`:
```
# Load myScripts
export PATH="$PATH:$HOME/myScripts"
```

## Note
The script is for UNIX systems and depends on Node.js
If you get a `Permission denied` when you try to execute the script,
you have to set the permission of the file using `chmod`.
Example: `chmod 755 file_name` (owner can read, write and execute - group and others can read and execute)
