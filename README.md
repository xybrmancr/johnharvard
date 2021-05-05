# John Harvard Bot
**Features in Progress:**
- Q&A Function - John Harvard automatically answers common questions 
- Harvard dictionary - e.g. yale = safety school
- Quote Book Function - certain messages are scraped into a book of quotes


**Notes from Original Developer:**
- Runs on a free Heroku account
- Required Heroku Environment Variables (Config Vars)
    - BOT_NAME` - The name of your bot
    - `gm_dev_group` - Group ID for the "Dev Room" chat (Format: XXXXXXXX)
    - `GM_DEV_BOT_ID` - Bot ID for the "Dev Room" chat (Format: XXXXXXXXXXXXXXXXXXXXXXXXXX)

    - `gm_primary_group` - Group ID for the chat group with your friends (Format: XXXXXXXX)
    - `GM_PRIMARY_BOT_ID` - Bot ID for the chat group with your friends (Format: XXXXXXXXXXXXXXXXXXXXXXXXXX)
- Local Testing

You can run `/app.py` to open a "chat prompt", simulate sending messages to Eclectus, and view its response. It doesn't simulate extracting the chat message from the data received by different messaging platforms, so this is mainly useful for testing your custom commands or new modules.
```
    $ python3 app.py
    Bot is ready. Press Ctrl+C to exit.
        Chat > Hello World!
                {'text': 'Hiya!'}
        Chat > Hello Eclectus Bot!
                {'text': "Hi, I'm a bot!"}
        Chat > Lets !flip a coin
                {'text': 'Dev flips a coin. It landed on heads!'}
```
