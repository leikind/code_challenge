# Code Challenge

### 1. Date periods

A date period has a start date and an end date, these days are part of the period.
Write a function which takes two date periods and returns one of the following:
* `[:no_intersection, older_date_period, newer_date_period]` - date periods do not intersect,
  it also returns both periods ordered in the ascending order.
* `[:includes, smaller_period, bigger_period]` - one date period is part of the other
  date period. The first returned period is the one which is part of the other bigger
  date period.
* `[:intersection, older_date_period, newer_date_period, intersection_period]` - one date period
  is part of the other date period.  The third date period is a new date period which is the
  intersection of the two.

### 2. Parentheses

Write a function which validates parentheses in a string. The number of open parentheses should
equal the number of closing parentheses, and all closing parentheses should appear *after* their
opening parentheses.

Examples:

* `"ewe ( wewer ( wefwe ) wefgf) "` - Valid
* `"ewe ) wewer ( "` - Invalid
* `"ewe ()) wewer ( ) "` - Invalid

### 3. Contractual year

A contract startes on a certain date. Write a function which, given a contract start date and
some other date in future, returns the number of the contractual year. That is, if a contract
starts on the January 2, 2014,  February 12, 2015 is contractual year 2. Let's assume the contract
is eternal.


### 4. Anagrams

You are given a list of English words. Write a function which takes a word and returns
a list of all words which are made of the same letters in a different order.

* "E" and "e" are the same letter
* "é" and "e" are two different letters
* Ignore spaces, dashes, and all non-alphanumeric characters

### 5. Anagram webservice

Write a simple webservice (using any framework of choice) which exposes the function from the previous assignment 
via a simple REST/JSON webservice.

### 6. Anagram webservice + RDBMS

We need to modify the anagram webservice to use it for the Martian language.
The Martian language  has 9,000,000,000,000 words, therefore we cannot keep our data
structures in memory. Please rewrite the webservice of assignment 5 using a relational database.


