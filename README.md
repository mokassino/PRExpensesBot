## Introduction
PRExpensesBot is a telegram bot that keep track of your expenses, bills, purchases and so on.
### What this bot can do:
* Add or delete items from the database
* For each item you can specify a group or category i.e "Food","Bills","Hobby"
* Subscribe/Unsubscribe function for automatic recaps 
* Multi-user compatible: if your friends or relatives want to use it, they can use your bot.
* Monthly and yearly recaps sorted by groups and months
# Requirements:
* [python 3.9.2](https://www.python.org/)
* [redis-server](https://redis.io/topics/quickstart)

## If you're new to redis or never used it:
If you just wanna try the bot once, you're fine with redis default configs
Otherwise, please be sure to read atleast [this](https://redis.io/topics/memory-optimization#memory-allocation). I'm actually testing it with a limit of 50mb; generally the more people use the same istance, the more the expenses amount to, the greater the limit needs to be. But chill, you're not running twitter, so it is unlikely that you will use tons of memory.
Please, keep your redis istance in [protected mode](https://redis.io/topics/security), it is enabled by default, so if you don't change anything in config you'll be ok. 

## Usage
1. [Create a new bot and get its telegram bot token](https://core.telegram.org/bots#creating-a-new-bot)
2. Download the code, edit ``bot.py`` inside the directory with your favorite editor
3. Insert your bot token inside the quotation marks ``MYTOKEN = " "``
4. [Install Redis, test it, config it](https://redis.io/topics/quickstart)
5. Run the server instance and the bot
6. Look for your bot on telegram and message him with /help to get the full list of commands

## License
Released under the [MIT License](LICENSE)
