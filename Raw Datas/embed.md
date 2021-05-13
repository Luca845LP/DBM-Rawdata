# Embed Command
--------------------
### [Command](https://github.com/Luca845LP/DBM-Rawdata/blob/main/Raw%20Datas/embed.md#command-1 "Click")

__Das ist ein Deutscher Embed Creator.__

Dieser Creator erstellt dir mit einem Menü einen Embed ohne einmal den Bot Maker zu Öffnen!

***__VOLL EINSTELLBAR__***
--------------------
## Command
```json
{
  "name": "embed",
  "permissions": "ADMINISTRATOR",
  "restriction": "1",
  "_id": "lkKEJ",
  "actions": [
    {
      "storage": "0",
      "varName": "msg1",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "🔨 **|** Wenn du den Embed Creator starten willst Reagiere mit 👍",
      "storage": "1",
      "varName2": "msg1",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "1",
      "varName": "msg1",
      "emoji": "4",
      "varName2": "👍",
      "varName3": "",
      "name": "Add Reaction"
    },
    {
      "storage": "1",
      "varName": "msg1",
      "filter": "reaction.emoji.name === '👍' && author.id === user.id",
      "max": "1",
      "time": "60000",
      "maxEmojis": "",
      "maxUsers": "",
      "iftrue": "2",
      "iftrueVal": "10",
      "iffalse": "0",
      "iffalseVal": "",
      "storage2": "0",
      "varName2": "",
      "name": "Await Reaction Call Action"
    },
    {
      "storage": "1",
      "varName": "msg1",
      "message": "🔨 **|** Embed Creator abgebrochen - Grund: Keine Reaktion",
      "storage2": "1",
      "varName2": "",
      "name": "Edit Message"
    },
    {
      "storage": "1",
      "varName": "msg1",
      "name": "Clear reactions from message"
    },
    {
      "time": "5",
      "measurement": "1",
      "name": "Wait"
    },
    {
      "storage": "1",
      "varName": "msg1",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "storage": "1",
      "varName": "msg1",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "🔨 **|** Sende die ID des Kanals wo der Embed gesendet werden soll. (Rechtsklick > ID Kopieren)",
      "storage": "1",
      "varName2": "msg2",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "60000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "5",
      "storage2": "1",
      "varName2": "r.a.channel",
      "name": "Await Response Call Action"
    },
    {
      "info": "0",
      "find": "${tempVars(\"r.a.channel\")}",
      "storage": "1",
      "varName": "a.channel",
      "name": "Find Channel"
    },
    {
      "storage": "1",
      "varName": "msg2",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "r.a.channel",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "🔨 **|** Sende die HEX Color ID des Embed's (Ohne #)",
      "storage": "1",
      "varName2": "msg3",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "60000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "5",
      "storage2": "1",
      "varName2": "r.a.color",
      "name": "Await Response Call Action"
    },
    {
      "message": "1",
      "varName": "r.a.color",
      "info": "2",
      "storage": "1",
      "varName2": "a.color",
      "name": "Store Message Info"
    },
    {
      "storage": "1",
      "varName": "msg3",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "r.a.color",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "🔨 **|** Sende mir den Embed Titel!",
      "storage": "1",
      "varName2": "msg4",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "60000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "5",
      "storage2": "1",
      "varName2": "r.a.titel",
      "name": "Await Response Call Action"
    },
    {
      "message": "1",
      "varName": "r.a.titel",
      "info": "2",
      "storage": "1",
      "varName2": "a.titel",
      "name": "Store Message Info"
    },
    {
      "storage": "1",
      "varName": "msg4",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "r.a.titel",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "🔨 **|** Sende mir die Embed Beschreibung!",
      "storage": "1",
      "varName2": "msg5",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "60000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "5",
      "storage2": "1",
      "varName2": "r.a.descr",
      "name": "Await Response Call Action"
    },
    {
      "message": "1",
      "varName": "r.a.descr",
      "info": "2",
      "storage": "1",
      "varName2": "a.descr",
      "name": "Store Message Info"
    },
    {
      "storage": "1",
      "varName": "msg5",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "r.a.descr",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "🔨 **|** Sende mir den Embed Footer! (Kein Footer = ´none´)",
      "storage": "1",
      "varName2": "msg6",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "60000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "5",
      "storage2": "1",
      "varName2": "r.a.footer",
      "name": "Await Response Call Action"
    },
    {
      "message": "1",
      "varName": "r.a.footer",
      "info": "2",
      "storage": "1",
      "varName2": "a.footer",
      "name": "Store Message Info"
    },
    {
      "storage": "1",
      "varName": "msg6",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "r.a.footer",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "🔨 **|** Überprüfe deine angaben und klicke danach auf 👍\n> Channel: ${tempVars(\"a.channel\")}\n> Farbe: ${tempVars(\"a.color\")}\n> Titel: ${tempVars(\"a.titel\")}\n> Beschreibung: ${tempVars(\"a.descr\")}\n> Footer: ${tempVars(\"a.footer\")}\n(Falls dir etwas nicht passt warte 20 Sekunden!)",
      "storage": "1",
      "varName2": "msg7",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "1",
      "varName": "msg7",
      "emoji": "4",
      "varName2": "👍",
      "varName3": "",
      "name": "Add Reaction"
    },
    {
      "storage": "1",
      "varName": "msg7",
      "filter": "reaction.emoji.name === '👍' && author.id === user.id",
      "max": "1",
      "time": "20000",
      "maxEmojis": "",
      "maxUsers": "",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "5",
      "storage2": "0",
      "varName2": "",
      "name": "Await Reaction Call Action"
    },
    {
      "storage": "1",
      "varName": "msg7",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "title": "${tempVars(\"a.titel\")}",
      "author": "",
      "color": "${tempVars(\"a.color\")}",
      "url": "",
      "authorIcon": "",
      "authorUrl": "",
      "imageUrl": "",
      "thumbUrl": "",
      "timestamp": "false",
      "debug": "false",
      "text": "",
      "year": "",
      "month": "",
      "day": "",
      "hour": "",
      "minute": "",
      "second": "",
      "storage": "1",
      "varName": "embed",
      "name": "Create Embed Message"
    },
    {
      "storage": "1",
      "varName": "embed",
      "message": "${tempVars(\"a.descr\")}",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "r.a.footer",
      "comparison": "5",
      "value": "'none'",
      "iftrue": "0",
      "iftrueVal": "1",
      "iffalse": "3",
      "iffalseVal": "1",
      "name": "Check Variable"
    },
    {
      "storage": "1",
      "varName": "embed",
      "message": "${tempVars(\"a.footer\")}",
      "footerIcon": "",
      "name": "Set Embed Footer"
    },
    {
      "storage": "1",
      "varName": "embed",
      "channel": "5",
      "varName2": "a.channel",
      "storage3": "0",
      "varName3": "",
      "iffalse": "0",
      "iffalseVal": "",
      "messageContent": "",
      "name": "Send Embed Message"
    }
  ]
}
```
