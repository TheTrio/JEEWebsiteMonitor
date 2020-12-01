# JEE Main Website Monitor

## What it does

This script constantly monitors the JEE Main website for changes and alerts the user when the website is changed. Its primary purpose is to automate the tedious task of constantly reloading the website, checking for exam results. 

## What it uses

This script uses `BeautifulSoup4` to access the HTML source code of the website, and checking its value with the source code 5 seconds ago. If the two match, the website hasn't changed. If they don't, the website has changed and the user is alerted using Telegram immediately. 

## How to reproduce

You must replace `CHAT_ID` and `TOKEN` with the Telegram chat id for your account and the API token for your bot respectively. Then, simply run the program. It is advised to run the program on a server to enhance performance. 

## Dependicies

1. [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/)
2. [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)
