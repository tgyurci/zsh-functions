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

## Functions

* aws-profile: Sets/unsets the AWS_PROFILE and AWS_SDK_LOAD_CONFIG env vars used
  by AWS clis and sdks
* docker-context: Sets/unsets the DOCKER_CONTEXT env var used by Docker cli
* cdg: Change up to the root directory of the current Git repository
* deattr: Remove common macOS extended attributes from a file
* mcd: mkdir + cd: Create a new directory and change to that
* prepend_path: Run a command with an additional directory at the first PATH
  element
* rrm: cd .. + rmdir: Change to the parent directory and remove the previous
  subdirectory
