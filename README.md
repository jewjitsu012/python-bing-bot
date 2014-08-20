python-bing-bot
===============

A bot for earning Bing Rewards on multiple accounts, written in Python.

This bot is based on work done on a Ruby project by TillerMiller.
https://github.com/TillerMiller/BingBot

The bot takes a YAML file as a configuration input, logs in to Facebook or Outlook, 
attempts to detect the number of searches needed for daily points, and then carries
out those searches systematically by either using faked input from the Faker class,
or hitting the iHeartQuotes API for a random quote.

What you need:

Google Chrome
Selenium Webdriver (Python) - http://docs.seleniumhq.org/download/
PyYAML - http://pyyaml.org
Faker - https://pypi.python.org/pypi/Faker/0.0.4

Unpack all archives and install them according to the directions given on each website.
On OSX this usually entails

cd /path/to/files
sudo python setup.py install

Config Setup:
Add email addresses to the config.yaml file as follows

FACEBOOK_EMAIL:
 - emailAddress
FACEBOOK_PASSWORD:
 - password
OUTLOOK_EMAIL:
 - emailAddress
OUTLOOK_PASSWORD:
 - password

Be mindful of the SPACE, DASH, SPACE before any config inputs
List as many emails as necessary (Bing has a 5 account per IP/household limit)


Usage
Mac, Linux : 

cd /path/to/PythonBingBot
python PBB.py
