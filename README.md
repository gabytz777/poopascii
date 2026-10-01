# poopascii

Print beautiful terminal ASCII art.

```
$ poopascii
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⡛⠛⠷⣶⣤⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⡇⠀⠀⠀⠙⠻⣷⣄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣾⠟⠀⠀⠀⠀⠀⠀⠈⣹⣿⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⣠⡴⠞⠉⠈⠻⣷⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
```

Or ask for something else entirely:

```
$ poopascii --list
alien
ass
bunny
...
whale
```

## Install

```sh
# Arch / AUR
paru -S poopascii
```

## Usage

| Command | What it does |
| --- | --- |
| `poopascii` | print the classic poop art |
| `poopascii --list` | list the available art names |
| `poopascii <name>` | print one specific piece, e.g. `poopascii whale` |
| `poopascii --random` | print a random piece |
| `poopascii --all` | print the whole collection with headers |
| `poopascii --help` | show the built-in help |

The `.txt` suffix is optional, and names are matched case insensitively.

Point `POOPASCII_ART_DIR` at your own directory of `.txt` files to use a custom
collection:

```sh
POOPASCII_ART_DIR=~/my-art poopascii --list
```

## The collection

26 pieces ship with the package, ranging from the braille poop classic to
whales, dinosaurs, aliens, pizza and more. Everything lives in `art/`, one
`.txt` file per piece, named after the piece.

`art/poop.txt` is the original piece shipped with poopascii. The rest come from
the [ASCII-Art-collection](https://github.com/joeky888/ASCII-Art-collection) and
are credited in [CREDITS](CREDITS).

## License

MIT, see [LICENSE](LICENSE). Note that the collected art predates this project
and is credited separately in [CREDITS](CREDITS).