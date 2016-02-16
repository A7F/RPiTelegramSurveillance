# Raspberry Pi room monitoring system

##Installing

once you installed Telegram client on your Raspberry, copy files in this repo to:

| Filename | Destination |
| --- | --- |
| `camera.sh` | `/home/pi/webcam/` |
| `action.lua` |`/home/pi/tg/` |

> please notice that you have to create folder *webcam*

Set sudo permissions using

```sudo chmod 777 /home/pi/webcam/camera.sh```

Run the script `action.lua` by using the following commands

```cd /home/pi/tg
bin/telegram-cli -k tg-server.pub -W -s action.lua```

##Issues known

1- does not overwrite older pictures

