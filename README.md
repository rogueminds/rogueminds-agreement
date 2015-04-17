# Working Agreement

## Instructions

* Install the Keybase command-line tool: [![](https://dl.dropboxusercontent.com/u/257359/static/img/download.png)][1]
* Switch to the proper date directory:

        cd 1999-12-31/

* Generate the agreement's checksum and store it in a file with your name:

        shasum -a 256 -p working-agreement.txt | awk '{ print $1 }' | tee signature-john-doe.txt

* Format the generated file like the following by adding the missing information (Full name and date of signature):

        John Doe
        1999-12-31 23:59 EDT
        deadbeefdeadbeefdeadbeefdeadbeefdeadbeefdeadbeefdeadbeefdeadbeef

* Sign the checksum file with the Keybase tool and save the output:

        keybase sign signature-john-doe.txt

* Commit only the generated `PGP ASCII Armored File` to the repository.

        git add signature-john-doe.txt.asc

## Revisions

[1]: https://keybase.io/docs/command_line/installation
