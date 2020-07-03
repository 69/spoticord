# fmcord `1.0.0`
**Display your current Last.FM song on Discord using the RPC API:**
![N|Solid](https://i.imgur.com/MXj59IH.png)

## Dependencies
  - NodeJS >=8
  - npm (>=5)
  - Discord
  - Git

## Setup

  - Clone the repo `git clone https://github.com/69/fmcord.git`
  - Install the modules `npm i`
  - Open Discord
  - Copy `config.json.example` to `config.json`
  - Set your last.fm username in the `config.json` file
  - Start the RPC app `node app.js`


## Useful links

* [RPC API Documentation](https://discordapp.com/developers/docs/topics/rpc)
* [Rich Presence Documentation](https://discordapp.com/developers/docs/rich-presence/how-to)

## Troubleshooting
### It says the song is being updated but it isn't being displayed on my profile?
  - Go to Discord settings
  - Go to "Games"
  - Make sure "Display currently running game as a status message" is ticked

### Invalid token function (or something similar)
  - Make sure your node is updated, you need at LEAST version 8.0.0!
  
### How to run in the background
  - Install pm2 `npm i pm2 -g`
  - Start the app `pm2 start app.js --name="fmcord"`
  - Use `pm2 log fmcord` to view the logs
  - Restart the app using `pm2 restart fmcord`
  - To stop it, run `pm2 stop fmcord`
