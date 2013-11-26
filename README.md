# rsink.sh

A backup utility for external hard drives that uses `rsync`.

In order to run `rsink.sh` you must set up your `.rsink/` directory. Inside this directory, there is a config file where your sources and destinations are listed. There is also a `profiles` directory, where you can manage settings for different backup schemes.

Refer to the To Do [wiki page] [1] for ideas on how you can help contribute to rsink.

## Installation

To install `rsink.sh`, open a terminal window and run the command: 

```
git clone https://github.com/adamlazz/rsink.git; cd rsink; chmod +x install.sh; ./install.sh`
```

## Configuration

The `config` file provides instructions for `rsync` on the source and destinations of your backups. Each line of the file is formatted like so:

```
profile source desintation exclude1 exclude2 ...

```

* There can be 0 or more excludes.
* There are space characters between the tokens in each line.
* There must be a new line at the end of the `config` file.

## Profiles

The `profiles` directory contains files that separate the 

Each profile file contains a list of options that rsync uses. For example, the `sink` profile uses rsync archive mode (`-a`) and lists the following options:

```
progress
a
ignore-existing
E

```

`rsink.sh` also comes with a `sync` profile for a source to destination sync. Files no longer on the source will be deleted from the destination. 

* For a full list of options run `man rsync`.
* You can name the profiles whatever you want.
* There must be a new line at the end of each profile file.

[1]: https://github.com/adamlazz/rsink/wiki/To-Do
