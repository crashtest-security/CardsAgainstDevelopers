Cards Against Developers
==========================

Cards Against Developers is based on [Cards Against Cryptography](https://github.com/CardsAgainstCryptography/CAC) and [Cards Against Humanity](https://cardsagainsthumanity.com/). It describes itself as "a party game for horrible people". Cards Against Developers is not quite as mean, but still has bit of an edge.

![Cards Against Developers Box](./images/box.png "Cards Against Developers Box")

Basic Rules
-----------

See [RULES.md](https://github.com/crashtest-security/CardsAgainstDevelopers/blob/master/RULES.md) for the rules.

License
-------

Cards Against Developers is shamelessly based on [Cards Against Cryptography](https://github.com/CardsAgainstCryptography/CAC) and [Cards Against Humanity](https://cardsagainsthumanity.com/), which were released under a Creative Commons BY-NC-SA 2.0 license (https://creativecommons.org/licenses/by-nc-sa/2.0/).

<img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/2.0/88x31.png" />

Cards Against Developers is released under the same license, which means you can use, remix, and share the game for free, but cannot sell it.

Contributing
------------

You can submit pull requests to propose new cards; see `src/black.txt` and `src/white.txt`.

Building
--------

The top-level Makefile can be used to recompile printable PDF and PNG versions of the cards:

    make PDFs PNGs

This should work on reasonable Linux or macOS systems. You need to have xelatex, python3, and ImageMagick's convert command in your path.

You can build specific releases of the cards using environment variables, e.g.

    make PDFs PNGs WHITE=white-extension BLACK=black-extension

Printed copies
--------------

Since Cards Against Humanity was released under a BY-NC-SA 2.0 license, the "non-commercial" aspect of that license implies that we cannot sell you a copy of this game. There may or may not be printed copies available as giveaways at events we attend.

You can make your own printed copy in three ways.

1. **Print at home.** Under the `PDFs-to-print` folder, there are printable PDFs of all the cards, formatted for 2-sided printing on either A4 or letter paper. You'll use up all the toner if print pages and pages of all-black backgrounds, so you should probably use the gray background. 
2. **Print at a local printshop.** You could also take the PDFs to your local print shop and have them print it on cardstock (80-pound or higher). Use a paper cutter to cut out the cards.
3. **Print via a commercial custom card manufacturer.** We printed our version of Cards Against Developers using MakePlayingCards.com. The folder `PNGs-to-print` contains the PNG images required to print a deck of cards at MakePlayingCards.com's [US Game Deck Size](https://www.makeplayingcards.com/design/custom-us-game-deck-size-cards.html), along with a [bi-fold (4 side) instruction booklet](https://www.makeplayingcards.com/pops/booklet-guide.html). At the time we wrote this, 1 set of cards, along with a booklet and plain white box, is $34.35 (US dollars), plus shipping (approximately $10 for standard shipping to most countries). Uploading the images and configure the project takes about 10 minutes.