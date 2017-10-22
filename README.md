# Bear Hunter - Alfred 3 Workflow
[![start with why](https://img.shields.io/badge/Download_Bear_Hunter-click_here-brightgreen.svg?style=flat)](https://github.com/oderwat/BearHunter/raw/master/Bear%20Hunter.alfredworkflow) [![Donate](https://img.shields.io/badge/Donate-PayPal-blue.svg)](https://www.paypal.me/oderwat/1) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


Lets you globally search for notes and use system wide hot-keys with the Bear notes taking application.

## Hot-Key

There is currently just one hot-key defined. It brings Bear to the front, resets it's state and focus the search field. You need to assign the key you want to use inside of the workflow. I personally use `Command+Alt+b` for the key combination.

## The global Bear Notes Search

* Use spaces to separate for any one of multiple words: 'this that'.
* Use quotes to search for the phrase: '"this that"'
* Use + to "require" a word: 'this +that'
* Use - to "exclude" a word: 'this -that'
* Use * to allow any characters in that place: #*/test (notes which have a subtag ending on test)

Remember that Bear stores its notes as raw markdown like text. Use this to your advantage in searches.

### Example 1:

`red yellow -green +apple`

Searches for all notes which containing the words "red" or "yellow" but not the word "green". And all of them must contain the word "apple".

> (red `or` yellow) `and not` green `and` apple

### Example 2:

`project +#work*/client1 +"mysql"`

Searches for all notes containing the words "project" and "mysql" having a tag that starts with "work" and ends with the subtag "client1"

### Example 3:

`[*.j*g] [*.png] [*.gif]`

Searches for all Notes containing a jpeg, gif or png image.

### Example 4:

` ```meta*saveas:*`

Searches for all notes with a [BearNanny](https://github.com/oderwat/BearNanny) saved code block :)
