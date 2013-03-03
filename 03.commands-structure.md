Commands Structure
===

There is a tradition in command structuring that most programs follow.

`command` `options` `argument`

- __Command__ is the command or program you are executing.
- __Options__ or __flags__
  - they are alphanumeric words.
  - there is two forms to flags
      - short form, which is a single dash followed by a short alphanumeric word (usually 1 character)
      - long form, which is a double dash followed by a alphanumeric word (usually human readable)
      - not all flags available in both forms.
      - e.g: `-h`, `--help` which are most common flags, that print command's help.
- __Argument__:
  - _Arguments_ usually are what the command will be applied upon
    - for example `cp` which copies files/dirs. need them spaced as argument.
      - `cp my-file.txt my-folder/my-file-copy.txt` here we have to arguments source and destination.
      - In most commands arguments for `source` Precedes `destination`

`command` `option argument` `argument`

- __Argumented flags__:
    - _flags_/_options_ can have there own arguments in such cases there argument must follow the flag.
    - for example `mkdir` command which makes directories have flag `-m` or `--mode` which take an argument to set the directories permission.
    - e.g: `mkdir --mode=711 my-dir/` or `mkdir -m744 my-dir/`
    - flags argument have to follow there flags they can be joined with the short form flag, separated by space or an equal sign '=' in both short or long forms.

`command` `options…` `arguments…`

`command` `options…` `argument` `arguments...`

- __Variable flags__
    - In most cases commands accepts variable count of _flags_.
        - Usually noted by `…` after the `[OPTIONS]` notation `[OPTION]…`, this means One or more _flag_ is optional.
        - Required _flags_ will be mentioned bare in the 'Usage' section of the help, as ``
- __Variable Arguments__
    - Some commands accepts variable count of _arguments_, some requires ablest one argument.
    - 