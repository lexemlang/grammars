# Lexem grammars

This repository is a collection of free-to-use [Lexem](https://github.com/lexemlang/lexem) grammars.

## Structure

The root directory contains the `grammar/` folder which contains all the available grammars. Each grammar is stored as a folder named with the lowercase name of the language. Inside them, there are always three elements: a **README.md** file specifying at least that the grammar is free to use and any other relevant data about the grammar, **the main grammar file**, named as `language.lxm` and **a folder called `tests`** containing at least one test to check the grammar is correct.

> **Note**: If the grammar is too complex it can be split in more `.lxm` files and folders under the language folder.

For example, the grammar folder structure for JSON can be like:

- grammars/
  - json/
    - README.md
    - json.lxm
    - tests/
      - test1.json
      - test2.json
      - ...
      
## Tester (In progress)

In the root folder of the project, it is included a file called `tester.sh` that allows to test a list of grammars specifying the lowercase name of the languages:

```sh
./tester.sh lang1 lang2 lang3
```

Or test all the grammars using the `all` flag:

```sh
./tester.sh -a
or
./tester.sh --all
```
