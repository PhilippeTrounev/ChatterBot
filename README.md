![Chatterbot: Machine learning in Python](https://i.imgur.com/b3SCmGT.png)

# ChatterBot

ChatterBot is a machine-learning based conversational dialog engine build in
Python which makes it possible to generate responses based on collections of
known conversations. The language independent design of ChatterBot allows it
to be trained to speak any language.

[![Package Version](https://img.shields.io/pypi/v/chatterbot.svg)](https://pypi.python.org/pypi/chatterbot/)
[![Requirements Status](https://requires.io/github/gunthercox/ChatterBot/requirements.svg?branch=master)](https://requires.io/github/gunthercox/ChatterBot/requirements/?branch=master)
[![Build Status](https://travis-ci.org/gunthercox/ChatterBot.svg?branch=master)](https://travis-ci.org/gunthercox/ChatterBot)
[![Documentation Status](https://readthedocs.org/projects/chatterbot/badge/?version=stable)](http://chatterbot.readthedocs.io/en/stable/?badge=stable)
[![Coverage Status](https://img.shields.io/coveralls/gunthercox/ChatterBot.svg)](https://coveralls.io/r/gunthercox/ChatterBot)
[![Code Climate](https://codeclimate.com/github/gunthercox/ChatterBot/badges/gpa.svg)](https://codeclimate.com/github/gunthercox/ChatterBot)
[![Join the chat at https://gitter.im/chatterbot/Lobby](https://badges.gitter.im/chatterbot/Lobby.svg)](https://gitter.im/chatterbot/Lobby?utm_source=badge&utm_medium=badge&utm_content=badge)

An example of typical input would be something like this:

> **user:** Good morning! How are you doing?  
> **bot:**  I am doing very well, thank you for asking.  
> **user:** You're welcome.  
> **bot:** Do you like hats?  

## How it works

An untrained instance of ChatterBot starts off with no knowledge of how to communicate. Each time a user enters a statement, the library saves the text that they entered and the text that the statement was in response to. As ChatterBot receives more input the number of responses that it can reply and the accuracy of each response in relation to the input statement increase. The program selects the closest matching response by searching for the closest matching known statement that matches the input, it then returns the most likely response to that statement based on how frequently each response is issued by the people the bot communicates with.

## Installation

This package can be installed from [PyPi](https://pypi.python.org/pypi/ChatterBot) by running:

```
pip install chatterbot
```

## Basic Usage

```
from chatterbot import ChatBot

chatbot = ChatBot(
    'Ron Obvious',
    trainer='chatterbot.trainers.ChatterBotCorpusTrainer'
)

# Train based on the english corpus
chatbot.train("chatterbot.corpus.english")

# Get a response to an input statement
chatbot.get_response("Hello, how are you today?")
```

# Training data

ChatterBot comes with a data utility module that can be used to train chat bots.
At the moment there is three languages, English, Spanish and Portuguese training data in this module. Contributions
of additional training data or training data in other languages would be greatly
appreciated. Take a look at the data files in the
[chatterbot-corpus](https://github.com/gunthercox/chatterbot-corpus)
package if you are interested in contributing.

```
# Train based on the english corpus
chatbot.train("chatterbot.corpus.english")

# Train based on english greetings corpus
chatbot.train("chatterbot.corpus.english.greetings")

# Train based on the english conversations corpus
chatbot.train("chatterbot.corpus.english.conversations")
```

**Corpus contributions are welcome! Please make a pull request.**

# [Documentation](https://chatterbot.readthedocs.io/)

View the [documentation](https://chatterbot.readthedocs.io/)
for ChatterBot on Read the Docs.

To build the documentation yourself using [Sphinx](http://www.sphinx-doc.org/), run:

```
sphinx-build -b html docs/ build/
```

# Examples

For examples, see the [examples](https://github.com/gunthercox/ChatterBot/tree/master/examples)
directory in this project's git repository.

There is also an example [Django project using ChatterBot](https://github.com/gunthercox/ChatterBot/tree/master/examples), as well as an example [Flask project using ChatterBot](https://github.com/chamkank/flask-chatterbot).

# History

See release notes for changes https://github.com/gunthercox/ChatterBot/releases

# Development pattern for contributors

1. [Create a fork](https://help.github.com/articles/fork-a-repo/) of
   the [main ChatterBot repository](https://github.com/gunthercox/ChatterBot) on GitHub.
2. Make your changes in a branch named something different from `master`, e.g. create
   a new branch `my-pull-request`.
3. [Create a pull request](https://help.github.com/articles/creating-a-pull-request/).
4. Please follow the [Python style guide for PEP-8](https://www.python.org/dev/peps/pep-0008/).
5. Use the projects [built-in automated testing](https://chatterbot.readthedocs.io/en/latest/testing.html)
   to help make sure that your contribution is free from errors.

# License

ChatterBot is licensed under the [BSD 3-clause license](https://opensource.org/licenses/BSD-3-Clause).
# Article <br> ######  test <br> To access **Docsie.io and its services** you must register a Docsie.io account by providing your **username and password**. If you *want to use paid features you must* provide **your full legal name**, current address, [phone number, a valid email address](https://docise.io), and any other `information indicated as required`. For more questions please contact admin@likalo.com.<br> ![login](https://images-na.ssl-images-amazon.com/images/G/01/lwa/btnLWA_gold_390x92.png "login")<br>[![](https://img.youtube.com/vi/XK2IRmlN7T8/0.jpg)](https://www.youtube.com/watch?v=XK2IRmlN7T8))<br>* test 1<br> * test 2<br> * **test** 3<br> * *test* 4<br> * [link](https://docise.io)<br> * **gdgdfg** *fsdfs* `fsdf  * da dasd ad `*<br> * <br> ```<br> `d*ef python:`*<br> ```<br> ```<br> `p*rint(1)`*<br> ```<br> ## We reserve the right to monitor any content on all accounts registered on our Sites, and your use of these Sites means you agree to this monitoring activity. This does indicate that any monitoring will take place on scheduled intervals or on any basis at all. <br> ## heading 2 <br> By registering or using our Sites you certify that you are at least 18 years old or at least the age of majority in the jurisdiction where you reside or from which you use this Site.<br> You acknowledge that Hanba.io will use the email address you provide as the primary method for communication.<br> You will provide truthful and accurate information about yourself upon registration; if your information changes at any time it is your responsibility to update your account to reflect these changes.<br> If you are assigned your account by an administrator, additional terms may apply to your use of the Sites, the administrator may revoke your access to the administered content at any time without further notice.<br> You are responsible for all activity and content such as photos, images, videos, graphics, written content, audio files, code, information, or data uploaded, collected, generated, stored, displayed, distributed, transmitted or exhibited on or in connection with your Account (“Materials”).<br> Do not share your account details for the Sites such as username and password with anyone, we are not liable for accounts compromised for any reason at all including malicious activity such as hacking, phishing, etc... If you believe your account has been compromised, please contact the administrator or info@likalo.com.<br>

