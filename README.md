# apertium-trunk

[Apertium][1] is a free/open-source platform for developing rule-based machine
translation systems.

This repository holds submodules to Apertium pairs that are in the [Apertium trunk][2].

To clone this repository with all its submodules, run

    git clone --recurse-submodules --shallow-submodules --depth 1 git@github.com:apertium/apertium-trunk.git

(Change `--depth 1` to `--depth N` to get the last N commits.)

Most users should not commit directly to this repository. All Apertium
repositories with the topic `apertium-trunk` are automatically updated in this
repository as submodules.

However, changes can be made to submodules in this repository after cloning it.
To make a commit to each changed submodule:

    git submodule foreach 'git commit -a -m <message>'
    git submodule foreach 'git push'

More information about using Git is [on the wiki][3]. More information about the
submodules is in the READMEs of those repositories under https://github.com/apertium.

[1]: https://wiki.apertium.org/
[2]: https://wiki.apertium.org/wiki/Trunk
[3]: https://wiki.apertium.org/wiki/Using_Git

## Compiling and installing

    $ ./autogen.sh
    $ PKG_CONFIG_PATH=~/apertium-trunk/build/share/pkgconfig/ ./configure --prefix=/home/tobeit/apertium-trunk/build
    $ make install

## Language pairs (Apertium)

Main page: https://wiki.apertium.org/wiki/Main_Page

List of language pairs: https://wiki.apertium.org/wiki/List_of_language_pairs

### Romanic

1. [x] Spanish <-\> Catalan             `2.2.0`
2. [x] French <-\> Catalan               `1.10.0`
3. [x] Spanish <-\> Portuguese      `1.1.6`
4. [x] Catalan <-\> Italian                `1.1.0`
5. [x] French <-\> Spanish             `0.9.4`
6. [x] Romanian <-\> Catalan        `1.0.0`
7. [x] Portuguese <-\> Catalan      `0.10.1`

### Nordic

1. [x] Swedish <-\> Danish             `0.8.1`
3. [x] Danish <-\> Norwegian        `1.5.1`
4. [x] Swedish <-\> Norwegian      `0.4.0`

### Slavic

1. [ ] Serbocroatian <-\> Slovenian              `Version`
2. [ ] Macedonian <-\> Bulgarian                 `Version`
3. [ ] Belarusian <-\> Russian                        `Version`
4. [ ] Russian <-\> Ukrainian                          `Version`