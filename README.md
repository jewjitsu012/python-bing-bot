python-bing-bot
===============

A bot for earning Bing Rewards on multiple accounts, written in Python.

This bot is based on work done on a Ruby project by . 

The bot takes a YAML file as a configuration input, logs in to Facebook or Outlook, 
attempts to detect the number of searches needed for daily points, and then carries
out those searches systematically by either using faked input from the Faker class,
or hitting the iHeartQuotes API for a random quote.

What you need:

Google Chrome
Selenium
PyYAML
Faker

Config Setup:


Usage
Mac, Linux : python PBB.py
