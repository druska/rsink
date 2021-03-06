# Changelog

## v0.2 (February 8, 2014)
* Bugfix: Multiple single character options print together
* Bugfix: Exit on Ctrl+C
* Feature: Check for unknown option and free space errors
* Feature: Comment lines and empty lines allowed in profiles
* Feature: Pushover support in .rsink/tools
* Feature: Single character options system
* Feature: [Pushover] [1] option (`-p` or `--pushover`)
* Feature: Dry-run (`-d` or `--dry-run`) option
* Feature: Help (`-h` or `--help`) option
* Feature: Silent (`-s` or `--silent`) option
* Feature: Version (`-v` or `--version`) option
* Feature: [Versioned backup] [2] profile using `rsync --link-dest`
* Feature: Constants stored in .rsink/constants.sh

## v0.1 (December 12, 2013)
* Initial release
* Automatic install
* `rsink.sh` with config and profiles
* OS X, Linux support

[1]: https://pushover.net/
[2]: http://blog.interlinked.org/tutorials/rsync_time_machine.html
