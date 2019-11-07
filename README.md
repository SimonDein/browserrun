# browserrun
A small script making it quick and easy to debug JavaScript files using your default browser's developer tools using a single command. No console.log'ing and Node.js's cumbersome debugger needed and you don't have to create or remember to delete cluttering html files just to use your browsers developer tools.

The script will handle the writing of a template html file for you and only one file will exist at a time. The file is deleted on startup or reboot. It will open the html file in your default program for handling html files - your browser.

All you have to do is pass the file to the command `browserrun` and a new tab is opened in your browser with the code running. Open your developer tools and you're ready.

## Install

### Clone the directory (fx. to a directory containing your scripts or git folders)
`git clone https://github.com/SimonDein/browserrun.git ~/myGitDirectory/browserrun`

Optional: Symlink the file to an appropriate destination (fx. where you keep your local commdand scripts)
`ln -s ~/myGitDirectory/browserrun/browserrun ~/myScripts`

### Add executable to path
add to `~/.bash_profile`:
```
# Load myScripts
export PATH="$PATH:$HOME/myScripts" (Path to dir of script)
```

## Example
`browserrun fileIWantToInspect.js` (tab opens witht the code running)
Open developer tools.


## Note
The script is for UNIX systems and depends on Node.js
If you get a `Permission denied` when you try to execute the script,
you have to set the permission of the file using `chmod`.
Example: `chmod 755 file_name` (owner can read, write and execute - group and others can read and execute)
