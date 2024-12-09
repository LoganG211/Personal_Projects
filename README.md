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


# Adding a new Repo

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
