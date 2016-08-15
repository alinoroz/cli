# cli

A simple telegram-bot wtitten in LUA based on [cli](https://github.com/alinoroz/cli)

# commands

 **sticker to photo**

`just send a sticker`

 **photo to sticker**

`just send a photo`

  **bold text**

`/bold text`

 **italic text**

`/italic text`

 **markdown link**

`/link url text`

**code text**

`/code text`

# channel

 **send bold text to a channel**

`/boldch @channelusername text`

 **send italic text to a channel**

`/italicch @channelusername text`

 **send markdown link to a channel**

`/linkch @channelusername url text`

**send code text to a channel**

`/codech @channelusername text`

# Installation

You should have [lua](http://www.lua.org/) installed

```bash
sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev libevent-dev make unzip git redis-server g++ libjansson-dev libpython-dev expat libexpat1-dev

```
`sudo apt-get install lua-socket` & `sudo apt-get install lua-sec`

Clone the bot

```
git clone https://github.com/alinoroz/cli.git

```

Then install bot using

`bash launch.sh install`

bot token in bot.lua (config part)

```lua

local bot_api_key = ""
local BASE_URL = "https://api.telegram.org/bot"..bot_api_key
local BASE_FOLDER = ""
```

And enter your telegram-id in admins table in [bot.lua](https://github.com/ali/cli)
```lua
local var = false
  local admins = {123456789,987654321}-- put your id here
  for k,v in pairs(admins) do

```

Save bot.lua

Start the bot

`lua bot.lua`
