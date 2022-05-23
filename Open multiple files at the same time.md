# Open multifle files ata the same time


## From the CLI

### Non-recursively

* To open multple html files in the cwd as tabs
```bash
$ vim -p *.html
```

* To open specific file in tabs
```bash
$ vim -p index.html default.html
```

### Recursively

To recursively open all `.html` files, adjust the wildcard to also target subdirectories:
```bash
$ vim -p **/*.html
```
This will start Vim and open one tab page for each .html file in the current working directory and all subdirectories (recursively).

## From within Vim - Option 1
---
Warning: The commands in option 1 will replace all tabs already open

### Non-recursively
To open multiple e.g. `.html` files in Vim from within Vim, in normal mode, enter the following two commands, one after the other:
```bash
:args *.html
:argdo tabe
```

`:args` list all `.html` files in the argument list. 
`:ardo` + `tabe` will open a new tabpage for each file in the argument list

To clear the argument list:
```bash
:argdelete
```

### Recursively

To open all `.html` files in the currect directory and all subdirectories (recursively), adjust the args command line to:
```bash
:args **/*.html
:argdo tabe
```

## From within Vim - Option 2

Notice: The following commands will not replace arguments or tabs which are already open.

### Non-recursively
```bash
:argadd *.html
:tab all
```

The :argadd command will add all .html files from the current working directory to the argument list. The :tab all command opens a new tabpage for all files in the argument list.

### Recursively
```bash
:argadd **/*.html
:tab all
```



