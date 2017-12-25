This project is a modified chrome-bisect-builds based on woxxom's changes.

woxxom's changes cache chrome builds so if you need to run the same bisect
multiple times you can do it without the script re-downloading the same files.

It also adds color:

[![color](screenshots/color.png?raw=true)](screenshots/color.png?raw=true)

Currently the woxxom modifications only work on Windows because of the changes
to the UnzipFilenameToDir function, at least.

Change SNAPSHOTS_DIR to a full path to cache the revisions and change SEVEN_ZIP
to the full path of 7z.exe.

Note the snapshots cache will grow big pretty fast. But if you need to run
the same bisect or revision repeatedly for
[some reason](https://bugs.chromium.org/p/chromium/issues/detail?id=770054#),
it's very helpful.

This woxxom branch also contains my modifications to the woxxom script that I
needed to get it running. The original woxxom script can be found
[here](https://bugs.chromium.org/p/chromium/issues/detail?id=783353#c3).
