# Sublime PHPUnit

Convenient Sublime Text commands for running your PHPUnit tests. Scans up the directory tree to find the closest
phpunit.xml file and runs phpunit from there. If it can't find one, it just runs phpunit from `/`.

## Installation

For now, you can run this on **Windows 10**. You should be able to run it on Windows 7/8 though I didn't test on those
versions.

Just `git clone` this repo into your `'C:\Users\<your_user>\AppData\Roaming\Sublime Text 3/Packages'` directory and
you're good to go.

You can find the commands in the command palette under "Sublime PHPUnit", or map any of these commands to whatever
shortcuts you want:

```
run_phpunit_test
run_phpunit_tests_in_dir
run_single_phpunit_test
run_all_phpunit_tests
```

By default, this package uses Window's cmd.exe application due to how `os.system` works in Python 3, for Windows. Read
[here](https://docs.python.org/3/library/os.html#os.system) to find out more.

## Future plans

- [ ] I'm currently investigating how one can use a different term for Windows in order to get colors.
- [ ] You should be able to specify a desired term using the `"phpunit-sublime-terminal": "ConEmu64"` configuration in your
settings.
- [ ] Support for Linux.

## Credits

[Implemention](https://github.com/adamwathan/sublime-phpunit) for MacOS by Adam Wathan.
