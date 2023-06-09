# ModBot
ModBot is a bot for viewing information from https://mod.io/

## Commands
* `/game <ID>` - Returns information about the game
* `/mod <Game_ID> <Mod_ID>`- Returns information about the game's mod
* `/subscribe <Game_ID>` - Subscribes your guild to mod updates
* `/unsubscribe <Game_ID>` - Unsubscribes your guild from mod updates

## Running localy
### Requirements
* `python 3.8 or higher`
### Installing
Clone this repository and install the packages from `requirements.txt`

You should also install an asynchronous driver for your SQL dialect

After that, modify the `config.yaml` file
```yaml
bot_token: "your discord bot token"
modio_api_key: "your modio api key"
db_uri: "dialect+async_driver://username:password@host:port/database"
test_guilds: [your bot test guilds ids]
```
And run the bot
```
python3 main.py
```

## Supported games
By default, you can only subscribe to update mods for 4 games:
* [Deep Rock Galatic](https://mod.io/g/drg)
* [Besiege](https://mod.io/g/besiege)
* [Space Engineers](https://mod.io/g/spaceengineers)
* [Insurgency: Sandstorm](https://mod.io/g/insurgencysandstorm)
