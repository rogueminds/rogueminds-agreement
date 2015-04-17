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

> [2014-11-07][2] – `b40a76187c2943cfb9960e161f09477e0ab43bc839e44fc0d47380972be555c8`  
> [2015-04-16][3] – `d44b962b362f21c5793a96ba4face1407a69c6828176b33c7f116ac1261b3978`  

[1]: https://keybase.io/docs/command_line/installation
[2]: 2014-11-07
[3]: 2014-04-16
