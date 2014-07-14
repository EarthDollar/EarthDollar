EarthDollar integration/staging tree
================================

http://www.EarthDollar.org
Copyright (c) 2011 Litecoin Developers

Copyright (c) 2014 Maplecoin Developers

Copyright (c) 2014 EarthDollar Developers

What is EarthDollar?
----------------

EarthDollar is a fork of MapleCoin using scrypt as a new proof-of-sustainability algorithm.


 - Name: EarthDollar - Version 0.8.1 BETA
 - Symbol: ED
 - Based on latest Litecoin/Maplecoin 0.8.1 source
 - Using Scrypt Mining
 - Block Target: 120 seconds
 - Difficulty Re-Targets every 4 blocks based on last 90 blocks (Quick Difficulty Readjustment)
 - Block reward: 305 ED halving every 10000000 blocks (approx. 38 years)
 - Total coin mined: 6.1 Billion ED
 - 6.1 billion coins will be mined in approx. first 150 years
 - Transaction Confirmations Needed: 6
 - Genesis Block Motto - "July 11, 2014: THE EARTH DOLLAR IS THE WORLD'S FIRST CURRENCY BACKED BY NATURAL CAPITAL, CONSISTING OF TREES, FRESH WATER, CARBON CREDITS AND BY LIFE ITSELF, SO THAT IS WHY WE CALL IT THE LIVING CURRENCY. HEREINAFTER YOU WILL FIND WORDS FROM OUR CORE TEAM MEMBERS WHY THEY JOINED THE EARTH DOLLAR PROJECT: [Love your neighbor as you love yourself. We are all one. - Ambassador David Kam the founder of the Earth Dollar hopes to bring Peace on Earth, and to heal the illusion of separation by reconnecting humanity back to the tree of life, which in turn will heal our biosphere and honor all our relations; the Earth Dollar was founded by David having a lucid dream, and vision in which he was asked to replant the tree of life] [Keepers of our Mother Earth ..... In nature we live, our HOME (Heal Our Mother Earth) (Algonquin translation: Ka kijigadimak ki-djodjo minan Aki.....ka-odjimadisiak, kidji mino madizimakik kidjodjo minan Aki) - Official Spokespersons for the Algonquin Nation of the Ottawa River Watershed - Charles T. Ratt and Tina Nottaway joined the project to bring true sovereignty to the Algonquin Nation and the Anicinabe People.] [it’s a beginning, to enhance protection for the forest and all it contains,,,,gladly i will like to join in this effort…i believe
…we as humans cannot live without it….and the time comes to educate others in this beautiful joint effort….migwetc - Louise Wawatie – Algonquin Elder of the Traditional Council of the Algonquin Nation.] [The Earth Dollar, is a currency based on the proof of sustainability and backed by natural capital, so as to allow all the economic models in their various corporate and governmental forms, to transition to a responsible and sustainable living economic system, while maintaining profitability, so that all can enjoy as a base, a living wage, while respecting what mother earth requires to sustain and promote life. Planting trees does not create a forest. We are all indigenous to this planet. For the ensured wellness of my son Migizi. Benoit Noël de Tilly - Waba Moko (White Bear) – Mother Earth Trust Ambassador and Algonquin Nation Liaison] [EarthDollar - A Coin For The Planet. A Money For The People - Master Coinmaker Anonymous Pirate] [For our next seven generations, live in Love and The Light together - Dixon de Leña, CEO of Mother Earth Trust] [In love we trust - Mark Anielski, Genuine Wealth Ambassador for Mother Earth Trust] [P.ROFITING E.ARTH R.ESPONSIBLY S.USTAINING O.UR N.ATURE – EARTH DOLLAR - Fish]  AMEN! AHO!!"
 

For more information, as well as an immediately useable, binary version of
the EarthDollar client sofware, see http://www.EarthDollar.org

License
-------

EarthDollar is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Litecoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion (if they haven't already) on the
[mailing list](http://sourceforge.net/mailarchive/forum.php?forum_name=bitcoin-development).

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of Litecoin.

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
    ./litecoin-qt_test

