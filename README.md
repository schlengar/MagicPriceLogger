# MagicPriceLogger

A simple tool to log the prices of selected cards of the card game Magic The Gathering.


## What it does

We store a list of card names in a local (text) file. Every 12 hours we look up the price of those cards on the following websites:
* US-American Sites:
    * [mtgStocks](https://www.mtgstocks.com/) (This site already aggregates over different sites and provides three average prices)
    * [TCG Player](http://www.tcgplayer.com/)
* European Sites:
    * [MagicCardMarket](https://www.magiccardmarket.eu/) (Well, to be fair, it's the only real one in Europe, being a marketplace itself and providing average prices)
    
We store the readouts and compute a weighted average for the US and the EU sites seperately, then we store these data points in a database.

## Why?

First of all, for practise. Second, as a player of the game, I'm interested in the market dynamics. Third, maybe there are interesting correlations between the US and EU prices which could be used to react to spikes in the market, *i.e.* to know when I should sell a card I have or buy one I want.
