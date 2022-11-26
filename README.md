# Xcode toolbox

Scripts to help me with my Xcode projects.  Consider all scripts tagged with
`WORKSFORME`.  😉  I'm not responsible for any damage caused by these scripts.


## Scripts

### xcconfig-version-bump
[`xcconfig-version-bump`](xcconfig-version-bump) sets the value for a given key
in a `.xcconfig` and commits the updated file to git.
[Fish](https://fishshell.com/) script.

I use it to automatically increment `CURRENT_PROJECT_VERSION` in the pre-build
step:

```bash
cd "${PROJECT_DIR}"
xcconfig-version-bump --file some.xcconfig --var CURRENT_PROJECT_VERSION --bump
```

Can also be used to set the value of a variable in a `.xcconfig` file:

```bash
xcconfig-version-bump --file some.xcconfig --var MARKETING_VERSION --set 1.2.3
```


## Author

Carlo Zottmann, <carlo@zottmann.co>, https://zottmann.co/,
https://github.com/czottmann


## License
```
        DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004

Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

Everyone is permitted to copy and distribute verbatim or modified
copies of this license document, and changing it is allowed as long
as the name is changed.

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
  TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

  0. You just DO WHAT THE FUCK YOU WANT TO.
```
