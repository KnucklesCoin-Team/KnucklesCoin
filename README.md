Knucklescoin
================================
	
![Downloads](	https://img.shields.io/github/downloads/KnucklesCoin-Team/KnucklesCoin/total.svg)
![Version](https://img.shields.io/github/tag/KnucklesCoin-Team/KnucklesCoin.svg)
![Release Date](	https://img.shields.io/github/release-date/KnucklesCoin-Team/KnucklesCoin.svg)
![Code Size](	https://img.shields.io/github/languages/code-size/KnucklesCoin-Team/KnucklesCoin.svg)
![Languages Count](	https://img.shields.io/github/languages/count/KnucklesCoin-Team/KnucklesCoin.svg)

Copyright (c) 2009-2014 Bitcoin Developers

Copyright (c) 2011-2014 Litecoin Developers

Copyright (c) 2017-2018 KnucklesCoin Developers

What is Knucklescoin?
----------------

Check out the subreddit, [https://www.reddit.com/r/KnucklesCoin](https://www.reddit.com/r/KnucklesCoin)

Knucklescoin is a alternative version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins

The rest is the same as Bitcoin.
 - 50 coins per block
 - 2016 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Knucklescoin client sofware, see this repo.

License
-------

Knucklescoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

### Usage

#### Linux

`./knucklescoin-qt` will run on Ubuntu. For other distributions it must be recompiled from source make sure you have installed all the dependencies, these can be found [here](https://pastebin.com/raw/s5bEu7cm) and copied into the Terminal. To compile and run:

    qmake
    make
    ./knucklescoin-qt

#### Windows

Coming soon. Final stage of packaging. Expected release 12th January 2018.

#### OSX

Coming soon. Compiling errors preventing build, developers welcome to try, will be released if successful.

### Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./knucklescoin-qt_test

