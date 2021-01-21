# git2package

**git2package** is a set of bash scripts that can download (clone) git source code repositories and compile them into packages using recipes that are written in bash script.

The recipes are not part of the git2package repo, but will be automatically downloaded from git repos.  Multiple recipe repos can be added from the "Configure git2package" dialog, and you can add a directory to the "recipes" directory with your own recipes too. (The format for an automatically downloaded repo is \<user name\>.\<repo name\> but you can use any directory name you want as long as it doesn't conflict with the auto downloaded ones.)

**git2package** will use gtkdialog if available for a nice user interface, but can also use ncurses or be used from the command line.

The default output directory is $HOME where the finished packages will be put along with log files, and the default working directory is /tmp/git2package/ but both of these can be configured from the "Configure git2package" dialog.


## Usage

**git2package** is a ROX-App, so if you use ROX-Filer as your file manager you can just click on it after downloading or cloning it.  If you do not use ROX-Filer you can start it by clicking on either the AppRun or git2package scripts inside the git2package directory.

The locations of the source code repositories are specified with the recipes and **git2package** will offer to clone them to the same location as the **git2package** AppDir, or you can choose another location.

**git2package** allows you to choose which git branch you want to compile from, or you can enter a specific commit hash.  If you are trying to compile the same branch or commit more than once, you may need to delete the temporary files in /tmp/git2package/ or wherever you set the location of the working directory.
