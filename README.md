## What ?

Another command line tool that lets you move faster between different
directories. 

## How ?

- Add the following line to your `.bashrc` pointing to the script directory

```bash
source $PATH_TO_SCRIPT/mark
```

- When in a directory that you want to mark, just type `mark`

- To list the marks, just type `mark ls`

- A number / index is assigned to each marks. which will be outputted when using `mark ls`

- To `cd` to a directory, type `mark cd <number>`

- Some aliases are defined for ease of use
  - `m` is an alias for `mark`
  - `mcd` is an alias for `mark cd`
  - `mls` is an alias for `mark ls`

**Example**

``` bash
[user@host ~/dev/scripts/project1 ]$ mark

[user@host ~/dev/scripts/project1 ]$ mls
1 /home/user/dev/repositories/project_x/src
2 /home/user/dev/scripts/project1 

[user@host ~/dev/scripts/project1 ]$ mcd 1

[user@host ~/dev/repositories/project_x/src ]$ 
```

**Changing location of `.mark` file**

- By default, the mark file is located in `$HOME/.mark`.
You can change this behaviour by modifying the `$MARK_FILE` environment variable