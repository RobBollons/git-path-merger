#GIT PATH MERGER

Move all the files from one location to another in git.

This was written to aid in resolving an issue where Windows git users with a case-insensitive file system would add files to a path that already exists but with a different case e.g:

Windows users: ./source/myFolder/lib.cpp
Linux users:   ./source/myfolder/lib.cpp

In the example both the files were intended be the same but are treated as seperate files by git due to the 'f' in 'myFolder' being a different case.

##DEPENDECIES
- Standard Unix tools (bash, echo, mkdir, find)
- Git

##INSTALLATION
Copy or symlink git-path-merger to your bin folder or a location in your path e.g. : `cp git-path-merger ~/bin/`

##USAGE

`$ git-path-merger ./source-folder ./destination-folder`


example:
`git-path-merger ./source/myFolder ./source/myfolder`
