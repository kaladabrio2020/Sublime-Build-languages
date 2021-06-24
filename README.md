# Sublime-Build-languages

- Running with cmd of windows 
- For languages :
        * Julia
        * Python
        * JavaScript
        * C#
        * C++
        * Html


1) Julia:

{
   "cmd": "start cmd /k julia $file_name",
   "file_regex": "^(...?):([0-9]):?([0-9]*)",
   "working_dir": "$file_path",
   "selector": "source.julia",
   "shell": true,
   "quiet": true
}


2) Python:

{
    "shell_cmd": "start cmd /k python $file_name",
    "selector": "source.python",
    "working_dir": "$file_path"
}



3) Javascript:
{
    "cmd": ["C:\\Program Files\\nodejs\\node.exe", "$file"],
    "selector": "source.js"
}

    *OR*
{
   "cmd": "start cmd /k node $file_name",
   "file_regex": "^(...?):([0-9]):?([0-9]*)",
   "working_dir": "$file_path",
   "selector": "source.js",
   "shell": true,
   "quiet": true
}


4) Html:
{
    "cmd": ["C:\\Program Files (x86)\\Google\\Chrome\\Application\\chrome.exe", "$file"]
}



5) Csharp:
{
   "cmd": ["csc", "$file_name", "&&", "start","cmd", "/k", "$file_base_name.exe"],
   "file_regex": "^(...?):([0-9]):?([0-9]*)",
   "working_dir": "$file_path",
   "selector": "source.cs",
   "shell": true,
   "quiet": true
}




6) C++:
{
    "cmd": ["g++.exe", "-std=c++11", "-o", "$file_base_name", "$file", "&&", "start", "cmd", "/c", "$file_base_name & echo. & echo. & pause"],
    "shell": true,
    "selector": "source.c++"
}