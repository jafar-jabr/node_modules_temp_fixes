It sometimes happens that node modules
packages come with some problems which you
don't have time to wait until the fix it
and release a new version
in this case, I suggest that you make 
the required fix by your self and to overwrite
the problematic file in packages.json "postinstall"
as fellows :

1- create a directory "preBuildFiles" in your project root

2- add this line at script section in packages.json
```cmd
"postinstall": "node preBuildFiles/index.js"
```


