# Personal_Projects

This is a repo containing links to Personal_Projects that I've worked on.

Specific project requriments would be listed in their own repos.


# Cloning the Project Directory

If you want to clone the entire directory with all of the projects, follow this step:

```$ git clone --recurse-submodules https://github.com/LoganG211/Personal_Projects.git```

If that doesn't work then follow the longer process:
```
$ git clone https://github.com/LoganG211/Personal_Projects.git
$ cd Personal_Projects
$ git submodule init
$ git submodule update
```


# Updating a Submodule

When you have changed a submodule with the subsequent add/commit/push, you must also change this parent directory as well. If you have not already pulled to fill out the submodules, please do so as it might create an error later when we try to commit. If you have already made changes and pushed to the submodule repo it will most likely request to merge.
```
$ cd path/to/Personal_Projects
$ git add path/to/submodule
$ git commit -m "Update <specific> submodule to latest commit"
$ git push
```
The parent repo will only lead to a specific commit of the submodule, by updating it will now lead to the most recent version.


# Adding a new Submodule

Make sure the repo has already been created in Github, and pushed.
1. Go to the local parent directory with link of the new repo copied.
2. In gitbash run the command ```$ git submodule add <repo-URL> path/to/submodule```
3. To init and get contents of the new submodule ```$ git submodule init``` and ```$ git submodule update```

Afterwards, remember to add the changes to reflect the new submodule:
```
$ git add .gitmodules path/to/submodule
$ git commit -m <message-here>
$ git push
```
