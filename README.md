# Zsh functions

Miscellaneous Zsh functions.

## Usage

Copy the files found in the `functions/` directory into `~/.zsh/functions`:

```sh
$ mkdir -p -- ~/.zsh/functions
$ cp -a -- functions/* ~/.zsh/functions/
```

Insert these lines into your `.zshrc`:

```zsh
fpath=(~/.zsh/functions $fpath)
autoload -Uz ~/.zsh/functions/*(.:t)
```

And finally restart your shell.
