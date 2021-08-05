# Shawn's Mark Text Fork

This is a fork of Mark Text that has automatic file reloading.

## Motivation

I needed something to render my markdown live as I wrote it in vim. I used to use Typora, but a Typora update broke the live reload feature for me. Because Typora is closed-source (shame on you, Typora), I made the switch to Mark Text.

Mark Text supports continuous live reload, but it requires user interaction. Upon detecting a change in a file, Mark Text gives the user a prompt to reload at the bottom of the application that must be interacted with in order to reload. This fork gets rid of that prompt and just reloads automatically upon detecting that the currently opened file has been updated.

## Installation

The build instructions are almost totally identical to the [build instructions over on the official documentation](https://github.com/marktext/marktext/blob/develop/docs/dev/BUILD.md).

First, clone the repository:

```
$ git clone https://github.com/shawnduong/marktext.git
```

Make sure you have all the additional development dependencies installed. A full list of dependencies if listed on the official documentation mentioned earlier.

Then, install the rest of the dependencies:

```
$ yarn install
```

Now build the binary.

```
$ yarn run build:bin
```

You can now run the compiled binary. It's located at `./build/linux-unpacked/marktext`. You now have a working copy of this fork!
