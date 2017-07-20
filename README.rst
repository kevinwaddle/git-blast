git-blast: show git branches sorted by last commit date
=======================================================

``git-blast`` (Branch LAST) shows git branches ordered by the date of the last commit::

    $ git blast
    * master 33 minutes ago
      some-feature 4 days ago [M]
      dev-branch 4 days ago
      legacy-branch 5 days ago [M]
      another-feature 4 months ago

    $ git blast -f iso
    * master 2017-04-17 07:12:21 -0400
      some-feature 2017-04-13 09:23:41 -0400 [M]
      dev-branch 2017-04-13 19:32:14 -0400
      legacy-branch 2017-04-12 09:03:26 -0400 [M]
      another-feature 2016-12-03 11:30:01 -0500

    $ git blast -h
    usage: git-blast [-h] [-f DATEFORMAT]

    show git branches sorted by last commit date

    optional arguments:
      -h, --help            show this help message and exit
      -f DATEFORMAT, --dateformat DATEFORMAT
                            A git date format: rfc, iso, default, rfc2822, etc.
                            Defaults to relative




Installation
============

With `Homebrew`__::

    $ brew install kevinwaddle/git-blast/git-blast

__ https://brew.sh/

Manually::

    $ curl https://raw.githubusercontent.com/kevinwaddle/git-blast/master/git-blast -O /usr/local/bin/git-blast
    $ chmod +x /usr/local/bin/git-blast
