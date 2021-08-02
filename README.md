# Success Motivational Quotes

#### A simple but amazing package having more than 2000 motivational quotes. Get amazing quotes categorized by author names and categories.

### Motivation

These quotes were collected for a mobile app I created with React Native. After the app developed, I realized there should be a package for quotes which can be used to get famous quotes. If you want to download the app, here is the **[link](https://play.google.com/store/apps/details?id=com.reactnativetemplatequotes)** for android users.

**Check [this](https://github.com/Sanan4li/success-motivational-quotes)** repository for source code of the package.

## Getting started

### Installation

```bash
 npm install success-motivational-quotes
```

## Usage

- **_getAllQuotes()_** method returns an array of objects containing all the quotes.

```js
const quotes = require("success-motivational-quotes");
console.log(quotes.getAllQuotes());
```

```json
[
  {
    "id": "0",
    "category": "Albert Einstein",
    "body": "Life is like riding a bicycle. To keep your balance you must keep moving.",
    "by": "Albert Einstein"
  },
  {
    "id": "1",
    "category": "Albert Einstein",
    "body": "The important thing is not to stop questioning. Curiosity has its own reason for existing.",
    "by": "Albert Einstein"
  },
  {
    "id": "2",
    "category": "Albert Einstein",
    "body": "No problem can be solved from the same level of consciousness that created it.",
    "by": "Albert Einstein"
  }
]
```

- **_getAllCategories()_** method returns an array of categories.

```js
const quotes = require("success-motivational-quotes");
console.log(quotes.getAllCategories());
```

```json
[
  "Albert Einstein",
  "Donald Trump",
  "Abraham Lincoln",
  "Anthony Robbins",
  "Brian Tracey",
  "Dale Carnegie",
  "Dennis Waitley",
  "Earl Nightingale",
  "Jim Rohn",
  "Mark Victor Hansen",
  "Napoleon Hill",
  "Norman Vincent Peale",
  "Ralph Waldo Emerson",
  "Robert H. Schuller",
  "Robert T. Kiyosaki",
  "Thomas Edison",
  "Thomas Jefferson",
  "W. Clement Stone",
  "Zig Ziglar",
  "Taking Action",
  "Adversity",
  "Attitude",
  "Think Big",
  "Goals",
  "Learning",
  "Persistence",
  "Preparation",
  "Taking Risks",
  "Work",
  "Motivational",
  "Bill Gates",
  "Elon Musk",
  "Leadership",
  "Business",
  "Inspirational",
  "Success",
  "New",
  "Random"
]
```

- **_getQuotesByCategory(category)_** method returns an array of objects having quotes of that category. Please note that **_category_** is case sensitive.

```js
const quotes = require("success-motivational-quotes");
console.log(quotes.getQuotesByCategory("Success"));
```

```json
[
  {
    "id": "1001",
    "category": "Success",
    "body": "The genius of money is not knowing everything, but rather, surrounding yourself with those who do.",
    "by": " Glen Purdy"
  },
  {
    "id": "1002",
    "category": "Success",
    "body": "I believe that the only courage anybody ever needs is the courage to follow your own dreams.",
    "by": "Oprah Winfrey"
  }
]
```

- **_getQuotesByAuthor(authorName)_** method returns an array of objects having quotes of a specific author. Please note that **_authorName_** is case sensitive.

```js
const quotes = require("success-motivational-quotes");
console.log(quotes.getQuotesByAuthor("Albert Einstein"));
```

```json
[
  {
    "id": "0",
    "category": "Albert Einstein",
    "body": "Life is like riding a bicycle. To keep your balance you must keep moving.",
    "by": "Albert Einstein"
  },
  {
    "id": "1",
    "category": "Albert Einstein",
    "body": "The important thing is not to stop questioning. Curiosity has its own reason for existing.",
    "by": "Albert Einstein"
  }
]
```

- **_getTodaysQuote()_** method returns an object containing a random quote from the quotes array.

```js
const quotes = require("success-motivational-quotes");
console.log(quotes.getTodaysQuote());
```

```json
{
  "id": "1002",
  "category": "Success",
  "body": "I believe that the only courage anybody ever needs is the courage to follow your own dreams.",
  "by": "Oprah Winfrey"
}
```

- **_getQuoteById(quoteId)_** method returns a quote with the id passed as parameter.

```js
const quotes = require("success-motivational-quotes");
console.log(quotes.getQuoteById(56));
```

```json
{
  "id": "56",
  "category": "Anthony Robbins",
  "body": "It not knowing what to do, it's doing what you know.",
  "by": "Anthony Robbins"
}
```

## Want to contribute?

I would love to merge all pull requests if someone wants to contribute to this package. Please make sure all quotes are in english language.

## License

**MIT &copy;**

## Thanks!

Thank you for being here! Please tag me on [twitter](https://twitter.com/Sanan4li) if you develop something with this package.
