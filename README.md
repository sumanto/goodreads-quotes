# quotes-goodreads

The Quotes Goodreads library exported as [Node.js](https://nodejs.org/) modules.
[![npm version](https://badge.fury.io/js/quotes-goodreads.svg)](https://badge.fury.io/js/quotes-goodreads)

📚 Easily get access to Goodreads quotes. This is a static list, and doesn't make connection to the Goodreads website.

### Installing

Using npm:
```
$ npm i --save quotes-goodreads
```

## Usage

In Node.js:
```javascript
// Load the module
const quotes = require('quotes-goodreads');

// Get a random Goodreads quote
console.log(quotes.getRandomStringQuote());
```

## API
### quotes.getRandomStringQuote()
Example: quotes.getRandomStringQuote();

Returns a random quote as String.

### quotes.getRandomStringQuoteWithAuthor()
Example: quotes.getRandomStringQuoteWithAuthor();

Returns a random quote as string, with author's name also added.

### quotes.getMostPopularQuotesString([number])
Example: quotes.getMostPopularQuotesString(2);

Gets the most popular quote, by rank. Ranking starts at 1. If no number is given, it responds with most popular quote.

### quotes.getMostPopularQuotesStringWithAuthor([number])
Example: quotes.getMostPopularQuotesStringWithAuthor(2);

Same as getMostPopularQuotesString([number]), but author's name is also added.

### quotes.quotesByAuthor(string)
Example: quotes.quotesByAuthor('Dr. Seuss');

Returns an array of quotes in string by the author. Substring of author's name also work.

## Built With

* [lodash](https://github.com/lodash/lodash) - A modern JavaScript utility library delivering modularity, performance & extras.
* Dataset originally copied from https://www.kaggle.com/akmittal/quotes-dataset

## Authors
Written by [sumanto](https://github.com/sumanto)
