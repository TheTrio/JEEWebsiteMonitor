# JEE Main Website Monitor

## What it does

This script constantly monitors the JEE Main website for changes and alerts the user when the website is changed. Its primary purpose is to automate the tedious task of constantly reloading the website, checking for exam results. 

## What it uses

This script uses `BeautifulSoup4` to access the HTML source code of the website, and checking its value with the source code 5 seconds ago. If the two match, the website hasn't changed. If they don't, the website has changed and the user is alerted using Telegram immediately. 

## How to reproduce

This program was written in 2020, and the JEE Mains website(https://jeemain.nta.nic.in/webinfo/public/home.aspx) may have changed by the time you're reading this. Since this program uses HTML to find relevant text, it is highly likely that even a small change in the structure of the webpage may break the code. Hence, some tinkering might be required to run this program correctly. 

You're also expected to have an API Token for your Telegram chat bot, and that is to be replaced with `API_TOKEN`. If you're not sure what that means, please read [this](https://www.siteguarding.com/en/how-to-get-telegram-bot-api-token) quick and easy tutorial.

## Dependicies

1. [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/)
2. [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)
