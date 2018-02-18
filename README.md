# replify

*Replify* is a simple and useful command-line tool to create a REPL (read-eval-print loop) for *any* command.

## Usage

    usage: ./repl PREFIX

This creates a REPL that executes your *PREFIX* + the string read from `STDIN` in each iteration.

Press `^D` to exit the REPL. Press `^L^M` or `^L^J` to clear the screen.

### Example

Note that `> git ` is part of the prompt.

    $ repl git
    > git init
    Initialized empty Git repository in /home/john/dev/tools/replify/.git/

    > git add repl

    > git commit -m 'First commit'
    [master (root-commit) 1171dfa] First commit
     1 file changed, 47 insertions(+)
     create mode 100755 replify

    > git status
    On branch master
    Untracked files:
      (use "git add <file>..." to include in what will be committed)

        README.md

    nothing added to commit but untracked files present (use "git add" to track)

    > git
