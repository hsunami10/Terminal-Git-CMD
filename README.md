<h1>How to use Git using Terminal (Mac) and Command Prompt (Windows)</h1>
<p>Download Git <a href="https://git-scm.com/downloads">here</a></p>
<p>Download SourceTree <a href="https://www.sourcetreeapp.com/">here</a></p>
<h2>General Commands for Mac Terminal (Unix)</h2>
<h3>Open terminal - Spotlight Search "Terminal" - Many commands similar to Linux</h3>
<ul>
	<li>ls -> list files and directories (not hidden)</li>
	<li>ls -a -> list all directories <strong>and</strong> files</li>
	<li>cd <i>[directory name]</i> -> change directory</li>
	<li>cd .. -> go to parent directory</li>
	<li>cd -> change directory to the current user directory</li>
	<li><i>command1</i> && <i>command2</i> -> runs 2 successive commands in one line</li>
	<li>mkdir <i>[directory name]</i> -> make directory</li>
	<li>rmdir <i>[directory name]</i> -> remove directory </li>
	<li>mv <i>[oldname] [newname]</i> -> change file name from old to new</li>
	<li>mv <i>[current] [new]</i> -> move file from current directory to new directory</li>
	<li>exit -> log out of terminal</li>
	<li>touch <i>[filename]</i> -> create a new file with filename</li>
	<li>rm {-rf} <i>[name]</i> -> remove specified directory or file</li>
	<li>* - option extension (ex. rm *.txt removes all files with extension .txt)</li>
	<li>open -a <i>[application_name] [filename]</i> -> opens <i>filename</i> with <i>application_name</i></li>
	<li>open -e <i>[filename]</i> -> opens the specified file in TextEdit</li>
	<li>open . -> open current directory on terminal</li>
	<li>clear -> clear screen</li>
	<li>TAB key -> autocompletion</li>
	<li><strong>Show Hidden Files</strong></li>
	<ul>
		<li>defaults write com.apple.finder AppleShowAllFiles TRUE</li>
		<li>killall Finder</li>
	</ul>
	<li><strong>Zip/Unzip Files</strong></li>
	<ul>
		<li>zip -r <i>[filename] [directory]</i> -> zip <i>[filename]</i>.zip into the <i>directory</i></li>
		<li>unzip <i>[filename]</i>.zip</li>
	</ul>
	<li><strong>Display Data of Normal Files</strong></li>
	<ul>
		<li>cat <i>[filename]</i> -> catenate, displays whole <i>filename</i></li>
		<li>less <i>[filename]</i> -> displays whole <i>filename</i> one screen at a time</li>
		<li>head <i>[filename]</i> -> displays first 10 lines of <i>filename</i></li>
		<li>tail <i>[filename]</i> -> displays last 15 lines of <i>filename</i></li>
		<li>grep {-i, -n} <i>[text] [file/files]</i> -> searches for <i>text</i> in the specified <i>file</i></li>
			<ul>
				<li>-i -> ignore case sensitive</li>
				<li>-n -> list line numbers</li>
			</ul>
	</ul>
	<li>sudo <i>[command]</i> -> run <i>[command]</i> as root administrator</li>
	<li>sudo -u <i>[user]</i> -> run command as user</li>
	<li>pwd -> (print working directory) lists path to the current directory</li>
	<li>man <i>[command]</i> -> lists the system manual for that <i>command</i></li>
	<li><strong>control c</strong> -> terminate the current process</li>
	<li>cp <i>[filename] [another directory]</i> -> copies file with <i>filename</i> to <i>another directory</i></li>
	<li>scp <i>[src] [dest]</i> -> (secure copy protocol) copies files from <i>src</i> to a <i>dest</i></li>
	<ul>
		<li>-r -> copy recursively</li>
	</ul>
	<li>scp <i>[remote file] [local directory]</i> -> copies <i>remote files</i> to the <i>local directory path</i></li>
	<li>make <i>[program name]</i>
	<ul>
		<li>executes a set of UNIX commands from a file (default is Makefile unless specified by the the -f option</li>
		<li>builds project into an executable file</li>
		<li>ex. make project2 - run makefile or Makefile</li>
		<li>ex. make -f altmake <i>[target files (left of colon in make file]</i> - use file named altmake</li>
		<li>Click <a href="https://www.dropbox.com/s/byhu66ycugljj5u/Make%20and%20Makefiles.pdf?dl=0" target="_blank">here</a> for more information on make and makefiles</li>
	</ul>
	<li>./<i>[executable]</i> -> run project in <strong>current directory</strong></li>
</ul>
<h3>EMACS</h3>
<ul>
	<li>emacs -nw <i>[filename].extension</i> -> create and edit a file with name <i>filename</i> and extension <i>extension</i> (don’t open a new window)</li>
	<li>emacs <i>[filename].extension</i> -> create and edit file (may open a new window)</li>
	<li><strong>control-w</strong> -> cut text</li>
	<li><strong>control-m & control-w</strong> -> copy text</li>
	<li><strong>control-y</strong> -> paste text</li>
	<li><strong>control-x & control-s</strong> -> save file</li>
	<li><strong>control-x & control-c</strong> -> exit EMACS</li>
</ul>
<h2>General Commands for Linux</h2>
<ul>
	<li>grep -RI <i>[term]</i> * -> searches "term" in multiple files</li>
	<li>wget <i>[link]</i></li>
	<li>sudo <i>[command]</i> -> executes the <i>command</i> as a root
	<li>.sh files -> runnable from shell</li>
	<li>xclip -sel clip < <i>[path to file]</i> -> copy content of file to clipboard</li>
	<li>sudo apt-get install <i>[package]</i>
	<li>gedit <i>[filename]</i> -> opens <i>filename</i> in the built in text editor</li>
	<li><strong>To make a .run file executable...</strong></li>
	<ul>
		<li>chmod +x <i>[filename]</i></li>
		<li>sudo sh <i>[filename]</i></li>
	</ul>
	<li><strong>Set Permissions</strong></li>
	<ul>
			   <li><strong>NOTE:</strong> u = user, g = group, o = others, r = 4 = read, w = 2 = write, x = 1 = execute.</li>
			   <li><strong>NOTE:</strong> View permissions by typing: ls -l. 1st 3: user, 2nd 3: group, last 3: others.</li>
			   <li>chmod <i>[u/g/o]=[r/w/x] filename</i> - set permissions. Ex: chmod g=rwx file.txt</li>
			   <li>chmod <i>[u/g/o]+/-[r/w/x] filename</i> - add / remove permissions. Ex: chmod g-x file.txt</li>
			   <li>chmod <i>3_digit_number</i> - set permissions. 1st digit: user, 2nd digit: group, 3rd digit: others.</li>
               <li>chmod +x <i>[filename]</i> - make a file an executable</li>
               <li><a href="https://chmodcommand.com/chmod-400/">chmod 400</a> <i>[filename]</i> - <strong>owner</strong> can read</li>
               <li><a href="https://chmodcommand.com/chmod-666/">chmod 666</a> <i>[filename]</i> - <strong>all</strong> can read and write</li>
               <li><a href="https://chmodcommand.com/chmod-700/">chmod 700</a> <i>[filename]</i> - <strong>owner</strong> can read, write, execute</li>
		<li><a href="https://chmodcommand.com/chmod-755/">chmod 755</a> <i>[filename]</i> - <strong>all</strong> can read and execute, <strong>owner</strong> can also write</li>
               <li><a href="https://chmodcommand.com/chmod-777/">chmod 777</a> <i>[filename]</i> - <strong>all</strong> can read, write, execute</li>
	</ul>
	<li>tar -zcvf <i>[foldername].tar.gz [folder]</i> -> create tar.gz file</li>
	<li>tar -xvzf <i>filename.tar.gz</i> -> extract tar.gz file</li>
</ul>
<h2>General Commands for Windows Command Prompt</h2>
<h3>Open Command Line - Windows search "cmd"</h3>
<ul>
	<li>dir -> list all directories <strong>and</strong> files</li>
	<li>cd <i>[directory name]</i> -> change directory</li>
	<li>cd .. -> go back one directory</li>
	<li>cd ../../ -> go back multiple directories</li>
	<li>mkdir <i>[directory name]</i> -> make directory</li>
	<li>rename <i>[oldname] [newname]</i> -> change file name from old to new</li>
	<li>exit -> quit out of CMD</li>
	<li>echo <i>[content]</i> > <i>[filename]</i> -> creates a file with content and specified name</li>
	<li>rd <i>[directory</i> -> remove specified directory</li>
	<li>del /f <i>filename</i> -> force delete specified file</li>
	<li>start <i>[application]</i> -> start the specified application</li>
	<li>cls -> clear screen</li>
	<li>&& -> executes multiple commands together on one line</li>
	<li>TAB key -> autocompletion</li>
</ul>
<hr>
<hr>
<hr>
<hr>
<hr>
<h2>Git Concepts and Useful Commands</h2>
<h3>There are 3 states in Git</h3>
<ol>
	<li>Working Directory: contains untracked and modified files, and will list them when <i>git status</i> is run</li>
	<li>Staging Directory: organize what you want to be committed to the repository</li>
	<li>Committed Files</li>
</ol>
<p>Therefore, using Git is very simple: Make changes to files on your local repository, <i>add</i> them to the staging directory, and <i>commit</i> them to the remote repository.</p>
<hr>
<h3>Add files to staging directory</h3>
<ul>
	<li>git add <i>[filename]</i> -> adds the specified file</li>
	<li>git add . -> adds all untracked files in the current directory</li>
</ul>
<h3>Remove files from staging directory</h3>
<ul>
	<li>git reset <i>[filename]</i> -> removes the specified file</li>
	<li>git reset -> removes <strong>all</strong> files from staging directory</li>
</ul>
<hr>
<h3>Remove Tracking Files / Directories</h3>
<ul>
	<li>git rm -r <i>[directory]</i></li>
	<li>git rm <i>[filename]</i></li>
</ul>
<hr>
<h3>Configuration</h3>
<ul>
	<li>git config --global user.name <i>[your name]</i></li>
	<li>git config --global user.email <i>[your email]</i></li>
	<li>git config --global core.editor "<i>editor_name</i>"</li>
	<li>git config --list -> lists all of the configuration values</li>
	<li>git config --global push.default current -> git push -u defaults the remote branch name to be the same name as your local branch</li>
</ul>
<hr>
<h3>How to ask for help</h3>
<ul>
	<li>git <i>[verb]</i> --help</li>
	<li>git help <i>[verb]</i></li>
	<ul>
		<li>ex. git help add</li>
		<li>ex. git config --help</li>
	</ul>
</ul>
<hr>
<h3>Making changes to code</h3>
<ul>
	<li>git diff <i>[path]</i>-> shows changes made, only <strong>tracked</strong>files</li>
	<li>git diff --cached -> shows changes made in newly created, untracked files. Only works when it's staged</li>
	<li><i>[any git diff command] > [filename].patch</i> -> stores modifications in a patch file</li>
	<li>git apply <i>[filename].patch</i> -> applies changes shown in the patch file to the current git workspace</li>
	<li>git status -> shows which <strong>files</strong> changed</li>
	<li>git stash -> store changes in a stack, and revert those changes</li>
	<li>git stash pop -> apply the most recent stash, and <strong>remove</strong></li>
	<li>git stash apply -> apply the most recent stash, and <strong>keeps it in the stash</strong></li>
	<li>git stash list -> list stashes stored</li>
</ul>
<hr>
<h3>Pulling and Pushing</h3>
<ul>
	<li><strong><i>When in a group collaboration, ALWAYS PULL BEFORE PUSHING</i></strong></li>
	<li><strong>git pull [remote] [branchname]</strong></li>
	<li>git pull origin master -> pull any changes from the <strong>master branch</strong></li>
	<li>git push origin master -> push changes made from local repository to the <strong>master branch</strong> of the remote repository </li>
	<li>git push origin +master -> force push</li>
</ul>
<hr>
<hr>
<hr>
<h2>Git Workflow and Common Commands</h2>
<h3>Start tracking an existing project</h3>
<ol>
	<li>Make an empty repository on GitHub</li>
	<li>git init -> initialize local repository in your project directory/folder</li>
	<li>git status -> shows which files are untracked/changed</li>
	<li>Create a README.md file and .gitignore file</li>
	<ul>
		<li>README.md shows the information of the repository</li>
		<li>.gitignore tells Git to ignore the specified file names in it</li>
	</ul>
	<li>git add .</li>
	<li>git commit -m <i>"insert detailed description of changes here"</i> -> commits files with a specific message</li>
	<li>git log -> see commit history</li>
	<li>git remote add origin <i>[remote repository URL]</i> -> add <strong>local repo</strong> to <strong>remote repo</strong></li>
	<li>git push -u origin master -> push changes to the repository named <strong>origin</strong> and its <strong>master branch</strong></li>
</ol>
<hr>
<h3>Start working on an already existing remote repository</h3>
<ol>
	<li>Make a new directory</li>
	<li>git clone <i>[remote repository URL] [where to clone]</i> -> clone a remote repository to a specified directory</li>
	<ul><li>If you're in the directory you want to be in, <i>[where to clone]</i> is not needed</li></ul>
	<li>git remote -v -> lists information on selected repository</li>
	<li>git branch -a -> lists all branches of the repository</li>
	<li>git remote rm origin -> removes remote repository</li>
</ol>
<hr>
<p>In a professional setting, there would be more than one branch (one for each "feature"), and for the final product, those branches would be <i>merged</i> into the <strong>master branch</strong>.</p>
<h3>Multiple Branches</h3>
<ol>
	<li>Create a branch for your part of the project</li>
	<li>git branch <i>[name of branch]</i> -> creates a new branch with a specified name</li>
	<li>git checkout <i>[name of branch</i> -> allows you to work on the branch</li>
	<li>git branch -a -> lists all branches in repository, the <strong>green</strong> one is the current branch you are on</li>
	<p><strong><i>ONCE CHANGES ARE MADE TO THE BRANCH...</i></strong></p>
	<li>git status</li>
	<li>git add .</li>
	<li>git commit -m <i>"message"</i> -> only commits to the local branch</li>
	<li>git push -u origin <i>[name of branch]</i> -> push branch to remote repo</li>
	<ul>
		<li>But the branch isn't merged with the master branch</li>
		<li>Once all branches are finalized, merge with the master branch</li>
		<li><strong><i>Switch to the master branch before merging</i></strong></li>
	</ul>
	<li>git checkout master</li>
	<li>git branch --merged -> shows which branches have been merged so far</li>
	<li>git merge <i>[name of branch]</i> -> merges the branch with the named branch</li>
	<li>Push changes to the remote master branch as usual</li>
</ol>
<h4>Rename Branch</h4>
<ol>
	<li><strong>Rename local branch</strong></li>
	<ul>
		<li>on branch: git branch -m <i>new-name</i></li>
		<li>not on branch: git branch -m <i>old-name new-name</i></li>
	</ul>
	<li><strong>Delete the old-name remote branch and push the new-name local branch:</strong> git push origin :<i>old-name new-name</i></li>
	<li>Switch to branch</li>
	<li>git push -u origin <i>new-name</i></li>
</ol>
<h4>Delete Branches</h4>
<ol>
	<li>git branch -d <i>[name of branch]</i> -> deletes the selected branch locally</li>
	<li>git push origin --delete <i>[name of branch]</i> -> deletes the selected branch remotely</li>
	<li>git push origin :<i>[name of branch]</i> -> deletes the selected branch remotely</li>
	<li>git branch | grep <i>[keyword]</i> | xargs git branch -D -> deletes all local branches that names contain <i>[keyword]</i></li>
</ol>
<h3>Branch/Merging Conflicts</h3>
<ul>
	<li>git pull - merges and fetches all branches</li>
	<li><i>if you see: <<<<<<<<<<< HEAD


CODE1

=========

CODE2

<<<<<<<<< (a bunch of numbers - commit ID):</i> this tells you to choose one version (CODE1 or CODE2) and stick with it</li>
	<li>fix conflicts in file</li>
	<li>use git add to mark conflicts as resolved</li>
	<li><h3>Git Rebasing</h3></li>
	<ul>
		<li>git rebase [origin] [branch] (test merge)</li>
		<li>git rebase --continue -> continue</li>
		<li>git rebase --abort -> abort rebase</li>
		<li>git rebase --skip -> skip patch</li>
	</ul>
</ul>
<h3>Squashing Commits</h3>
<p>This is to make repositories more clean, squashing multiple commits into one commit.</p>
First, rebase with master:
<ul>
	<li>git checkout master</li>
	<li>git pull origin master</li>
	<li>git checkout <i>[branch-name]</i></li>
	<li>git rebase -i master</li>
</ul>
You should see a list of commits, each commit starting with the word "pick".<br>
Make sure the first commit says "pick" and change the rest from "pick" to "squash". -- This will squash each commit into the previous commit, which will continue until every commit is squashed into the first commit.<br>
Save and close the editor (vim - esc + w + q + enter)<br>
It will give you the opportunity to change the commit message.<br>
Save and close the editor again.<br>
Then you have to force push the final, squashed commit: git push --force-with-lease origin.
<h3>Undoing - Mistakes</h3>
<ul>
	<li>See state IDs and history -> git reflog</li>
	<li>Revert back to past commit -> git reset --hard [commitId] && git clean -f</li>
	<li>Undo commit (before push) -> git reset HEAD~ -> undo recent commit</li>
</ul>
<h3>Completely Overriding Local Files</h3>
<ul>
	<li>git fetch --all</li>
	<li>git reset --hard [remote]/[branch_name]</li>
</ul>
