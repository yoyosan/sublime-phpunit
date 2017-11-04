# Sublime PHPUnit

Convenient Sublime Text commands for running your PHPUnit tests. Scans up the directory tree to find the closest
phpunit.xml file and runs phpunit from there. If it can't find one, it just runs phpunit from `/`.

## Installation

For now, you can run this on **Windows 10** and **Linux**. You should be able to run it on Windows 7/8 though I didn't
test on those versions.

### Windows

```
git clone git@github.com:yoyosan/sublime-phpunit.git 'C:\Users\<your_user>\AppData\Roaming\Sublime Text 3/Packages'
```

Note that, by default, this package uses Window's `cmd.exe` application due to how `os.system` works in Python 3, for Windows. Read
[here](https://docs.python.org/3/library/os.html#os.system) to find out more.

Therefore, there **won't be any colouring** of the output :(

### Linux

```
$ git clone git@github.com:yoyosan/sublime-phpunit.git /home/`whoami`/.config/sublime-text-3/Packages
# install terminator package
# Fedora
$ sudo dnf install terminator -y
# Ubuntu
$ sudo apt-get install terminator -y
```

Re/start Sublime.

### Shortcuts

You can find the commands in the command palette under "Sublime PHPUnit", or map any of these commands to whatever
shortcuts you want:

```
run_phpunit_test
run_phpunit_tests_in_dir
run_single_phpunit_test
run_all_phpunit_tests
```

## Future plans

- [X] Support for Linux.
- [X] Refactor code a bit.
- [X] Add support for running tests with a data provider.

## Credits

[Implemention](https://github.com/adamwathan/sublime-phpunit) for MacOS by Adam Wathan.
