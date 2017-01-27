# pyredictit
=======

pyredictit is a wrapper for the public PredictIt API (https://predictit.freshdesk.com/support/solutions/articles/12000001878-does-predictit-make-market-data-available-via-an-api-).  Running this module requires mechanicalsoup and <b>Python 3.6</b>.

**this can buy or sell shares using the money currently in your account. i am not responsible for any awful (or brilliant) trades you may accidentally or purposefully make with this wrapper. don't risk more than you can afford to lose. **

Things you can do with this currently are:
- Buy or sell shares of contracts that you already own.
- Check your current balance
- Find out how much you'd make if you sold all of your shares in a market
- Find out what you would make (or lose) depending on how the contract resolves
- Summarize all of your current contracts.
- Look up & purchase shares of contracts you don't currently own

UPDATE 1/26/2017 - the number 1 question I've been getting about this is "will it steal my login and password," and the answer is *of course not*, <b>but don't take my word for it!</b> Lines 202-213 are the parts where authentication is handled specifically, and I suspect that even people who don't fully understand Python's syntax will be able to see and verify for themselves that this information isn't transmitted anywhere beyond PI's server.

INSTALLATION:

1. Go to https://www.python.org/downloads/

2. Click "Download Python 3.6.0"

3. Install it and check "Add Python to PATH"  box in setup options.

4. Open up Powershell/Terminal and type: python -m pip install mechanicalsoup

5. Clone this repo

6. Use it like a Python module!

TODO:
* C O M M E N T S
* UNIT TESTS
* DOC TESTS
* Check volumes and current prices
* Custom Exception classes
* setup.py script
* Adding to pip
* stop loss and buy-at functionality - on hold, waiting for clarification from PI regarding automated trading.
* <s>Look up & purchase shares of contracts you don't currently own</s> - added 1/25/2017!

HOW YOU CAN HELP:

report all exceptions!  Include as much info as possible and please check to make sure that you are using valid login info and whatnot if you're copying over from the examples.  Also, *any* feedback is useful! 

WARNINGS <b>updated 1/27/2017</b>:
I've contacted PI about this and they say that the only things that are problematic in this wrapper is the calls to non-API data, like the login auth stuff.  So, I'm going to be commenting out those methods - be aware that removing the # sign before the comment re-enables the methods, so if you want to be in compliance with the TOS, leave those commented out!

