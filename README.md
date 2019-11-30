Graincoin integration/staging tree
================================

https://www.graincoin.com.br

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Litecoin Developers
Copyright (c) 2019 Graincoin Developers
What is Graincoin?
----------------

Graincoin is a decentralized cryptocurrency used for settling its value commodities, and actual use as seeds, the idea being that each unit is worth seeds that are planted in our fields and thus from the flutes and at a certain time of year is harvested in the so-called harvest day ”where you can sell for a much higher value.
Think of yourself as an investor, because in general, the purchase of our crypto resembles an investor, who buys a stock in the hope that it will appreciate.
With the difference that our cryptocurrencies are much more likely to appreciate since our allticoin has a very strong ballast that are the seeds, these seeds vary by market, for example if maize is more valued then we grow corn if it is beans then we plant beans or soybeans and so on, always in order to meet market demand.Graincoin is similar to Bitcoin, some differences are listed here.

 - subsidy halves in 440k blocks (~2 years)
 - ~64 million total coins
 - 50 coins per block
 - 400 blocks to retarget difficulty

Graincoin is a graincoin fork and almost everything is the same as graincoin, with some modifications made to further streamline transactions.

For more information, as well as an immediately useable, binary version of
the Graincoin client sofware, see https://www.graincoin.com.br.

License
-------

Graincoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Graincoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/graincoin-project/graincoin/tags) are created
regularly to indicate new official, stable release versions of Graincoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./graincoin-qt_test

