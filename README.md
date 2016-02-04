# ZSH EnvDir

The script allows to customise the `env` per folder.
Just drop a file named `.envrc` into a folder and add there your variables.
The script will automatically source the file when entering the folder and revert to the old `env` when exiting

## Installation

#### 1. Clone the repository:

```sh
git clone https://github.com/ganglio/envdir.git ~/.envdir
```

#### 2. Add `envdir` to your shell

```sh
echo "source ~/.envdir/envdir" >> .zshrc
```

## Functions

* `pushs` Pushes $1 to the stack
* `pops` Pops from stack. If $1 is provided the head of the stack is assigned to the $1 echoed otherwise
* `gets` Get the ${1}th element from the stack without changing the stack
* `sizes` Returns the size of the stack
* `has_envrc` Checks if the provided folder is enved. If no folder is provided checks the current folder
* `pipeset` Assigns stdin to $1
* `flushenv` Flushes the env
* `pushenv` Pushes the env on the stack
* `popenv` Pops the env from the stack

## Development

The source code is [hosted on GitHub](https://github.com/ganglio/envdir). It's pretty simple and easy to understand.

Please feel free to submit pull requests and file bugs on the [issue tracker](https://github.com/ganglio/envdir/issues).
