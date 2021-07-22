# Bot

# FOR TERMUX/UBUNTU/SSH USER
apt update && apt upgrade
apt install git -y
apt install nodejs -y
apt install ffmpeg -y
apt install imagemagick -y
git clone https://github.com/Nurutomo/wabot-aq
cd wabot-aq
npm install
npm update

# FOR WINDOWS/VPS/RDP USER
Download And Install Git Click Here
Download And Install NodeJS Click Here
Download And Install FFmpeg Click Here (Don't Forget Add FFmpeg to PATH enviroment variables)
Download And Install ImageMagick Click Here
git clone https://github.com/Nurutomo/wabot-aq
cd wabot-aq
npm install
npm update

Run
node .

# Arguments node . [--options] [<session name>]
--self
Activate self mode (Ignores other)

--pconly
If that chat not from private bot, bot will ignore

--gconly
If that chat not from group, bot will ignore

--swonly
If that chat not from status, bot will ignore

--prefix <prefixes>
prefixes are seperated by each character Set prefix
--server
Used for heroku or scan through website

--db <json-server-url>
Use external db instead of local db, Example Server https://json-server.nurutomo.repl.co/ Code: https://repl.it/@Nurutomo/json-server

node . --db 'https://json-server.nurutomo.repl.co/'

The server should have like this specification

# GET
GET /
Accept: application/json

# POST
POST /
Content-Type: application/json

{
 data: {}
}
--big-qr
If small qr unicode doesn't support

--restrict
Enables restricted plugins (which can lead your number to be banned if used too often)

Group Administration add, kick
--img
Enable image inspector through terminal

--autoread
If enabled, all incoming messages will be marked as read

--nyimak
No bot, just print received messages and add users to database

--test
Development Testing Mode

--trace
conn.logger.level = 'trace'

--debug
conn.logger.level = 'debug'
