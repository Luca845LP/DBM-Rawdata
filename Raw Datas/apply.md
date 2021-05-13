# Apply Command
--------------------
### [Command](https://github.com/Luca845LP/DBM-Rawdata/blob/main/Raw%20Datas/apply.md#command-1 "Click")

__Das ist ein Deutsches Bewerbungs System.__

Die Fragen sind:
- *Wie heißt Du?*
- *Wie alt bist du?*
- *Erzähl etwas Über Dich!* 
- *Was sind deine Erfahrungen / Referenzen?* 
- *Wie erreichen wir dich(Kontakt)?* 
- *Noch Weitere Infos / Anliegen? Schreib sie mir!*
- Das System macht für jeden User einen eigenen Channel damit man seine Ruhe hat und löscht diesen Automatisch und schickt einen Embed an einen Log Channel! 
- ***__VOLL EINSTELLBAR__***
--------------------
## Command
```
{
  "name": "<font color=\"orange\"> Global Chat </font>",
  "permissions": "NONE",
  "restriction": "1",
  "_id": "JhNwr",
  "actions": [
{
  "name": "apply",
  "permissions": "NONE",
  "restriction": "1",
  "_id": "ldrhY",
  "actions": [
    {
      "member": "1",
      "varName": "",
      "info": "2",
      "storage": "1",
      "varName2": "namee",
      "name": "Store Member Info"
    },
    {
      "member": "1",
      "varName": "",
      "info": "0",
      "storage": "1",
      "varName2": "author",
      "name": "Store Member Info"
    },
    {
      "comment": "<strong>Kategorie ID Einsetzen</strong>",
      "color": "#ff0000",
      "name": "Comment"
    },
    {
      "channelName": "🎬»${tempVars(\"namee\")}",
      "topic": "",
      "position": "",
      "storage": "1",
      "varName": "channel",
      "categoryID": "???",
      "reason": "",
      "name": "Create Text Channel"
    },
    {
      "comment": "----------------------------------------",
      "color": "#ff0000",
      "name": "Comment"
    },
    {
      "type": "1",
      "targetType": "2",
      "bitFields": "",
      "storage": "1",
      "varName": "allowed",
      "ADMINISTRATOR": null,
      "CREATE_INSTANT_INVITE": "Disallow",
      "KICK_MEMBERS": null,
      "BAN_MEMBERS": null,
      "MANAGE_CHANNELS": "Disallow",
      "MANAGE_GUILD": null,
      "ADD_REACTIONS": "Allow",
      "VIEW_AUDIT_LOG": null,
      "PRIORITY_SPEAKER": null,
      "STREAM": null,
      "VIEW_CHANNEL": "Allow",
      "SEND_MESSAGES": "Allow",
      "SEND_TTS_MESSAGES": "Allow",
      "MANAGE_MESSAGES": "Disallow",
      "EMBED_LINKS": "Allow",
      "ATTACH_FILES": "Allow",
      "READ_MESSAGE_HISTORY": "Allow",
      "MENTION_EVERYONE": "Disallow",
      "USE_EXTERNAL_EMOJIS": "Allow",
      "VIEW_GUILD_INSIGHT": null,
      "CONNECT": null,
      "SPEAK": null,
      "MUTE_MEMBERS": null,
      "DEAFEN_MEMBERS": null,
      "MOVE_MEMBERS": null,
      "USE_VAD": null,
      "CHANGE_NICKNAME": null,
      "MANAGE_NICKNAMES": null,
      "MANAGE_ROLES": null,
      "MANAGE_WEBHOOKS": "Disallow",
      "MANAGE_EMOJIS": null,
      "name": "Create Permissions"
    },
    {
      "type": "1",
      "targetType": "2",
      "bitFields": "",
      "storage": "1",
      "varName": "disallowed",
      "ADMINISTRATOR": null,
      "CREATE_INSTANT_INVITE": "Disallow",
      "KICK_MEMBERS": null,
      "BAN_MEMBERS": null,
      "MANAGE_CHANNELS": "Disallow",
      "MANAGE_GUILD": null,
      "ADD_REACTIONS": "Disallow",
      "VIEW_AUDIT_LOG": null,
      "PRIORITY_SPEAKER": null,
      "STREAM": null,
      "VIEW_CHANNEL": "Disallow",
      "SEND_MESSAGES": "Disallow",
      "SEND_TTS_MESSAGES": "Disallow",
      "MANAGE_MESSAGES": "Disallow",
      "EMBED_LINKS": "Disallow",
      "ATTACH_FILES": "Disallow",
      "READ_MESSAGE_HISTORY": "Disallow",
      "MENTION_EVERYONE": "Disallow",
      "USE_EXTERNAL_EMOJIS": "Disallow",
      "VIEW_GUILD_INSIGHT": null,
      "CONNECT": null,
      "SPEAK": null,
      "MUTE_MEMBERS": null,
      "DEAFEN_MEMBERS": null,
      "MOVE_MEMBERS": null,
      "USE_VAD": null,
      "CHANGE_NICKNAME": null,
      "MANAGE_NICKNAMES": null,
      "MANAGE_ROLES": null,
      "MANAGE_WEBHOOKS": "Disallow",
      "MANAGE_EMOJIS": null,
      "name": "Create Permissions"
    },
    {
      "comment": "<strong>Everyone ID Einsetzen</strong>",
      "color": "#ff0000",
      "name": "Comment"
    },
    {
      "info": "0",
      "find": "???",
      "storage": "1",
      "varName": "everyone",
      "name": "Find Role"
    },
    {
      "comment": "----------------------------------------",
      "color": "#ff0000",
      "name": "Comment"
    },
    {
      "target": "1",
      "way": "0",
      "storage": "3",
      "varName3": "channel",
      "role": "2",
      "varName": "",
      "member": "2",
      "varName2": "author",
      "storage3": "1",
      "varName4": "allowed",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Set Channel Permissions"
    },
    {
      "target": "0",
      "way": "0",
      "storage": "3",
      "varName3": "channel",
      "role": "3",
      "varName": "everyone",
      "member": "2",
      "varName2": "author",
      "storage3": "1",
      "varName4": "disallowed",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Set Channel Permissions"
    },
    {
      "storage": "0",
      "varName": "",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "member": "1",
      "varName": "",
      "info": "2",
      "storage": "1",
      "varName2": "membererr",
      "name": "Store Member Info"
    },
    {
      "channel": "5",
      "varName": "channel",
      "message": "${member}",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "title": "<:welt:730838974855118888> Bewerben",
      "author": "",
      "color": "5900ff",
      "url": "",
      "authorIcon": "",
      "authorUrl": "",
      "imageUrl": "",
      "thumbUrl": "",
      "timestamp": "true",
      "debug": "false",
      "text": "",
      "year": "",
      "month": "",
      "day": "",
      "hour": "",
      "minute": "",
      "second": "",
      "storage": "1",
      "varName": "applymsg",
      "name": "Create Embed Message"
    },
    {
      "storage": "1",
      "varName": "applymsg",
      "message": "Schön das du dich bei uns Bewerben willst!\nKlicke auf 👍 um die Bewerbung zu Starten",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "applymsg",
      "message": "Der Channel Löscht sich Automatisch!",
      "footerIcon": "",
      "name": "Set Embed Footer"
    },
    {
      "storage": "1",
      "varName": "applymsg",
      "channel": "5",
      "varName2": "channel",
      "storage3": "1",
      "varName3": "applymsggdd",
      "iffalse": "0",
      "iffalseVal": "",
      "messageContent": "",
      "name": "Send Embed Message"
    },
    {
      "storage": "1",
      "varName": "applymsggdd",
      "emoji": "4",
      "varName2": "👍",
      "varName3": "",
      "name": "Add Reaction"
    },
    {
      "storage": "1",
      "varName": "applymsggdd",
      "filter": "reaction.emoji.name === '👍' && author.id === user.id",
      "max": "1",
      "time": "120000",
      "maxEmojis": "",
      "maxUsers": "",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "1",
      "iffalseVal": "",
      "storage2": "0",
      "varName2": "",
      "name": "Await Reaction Call Action"
    },
    {
      "storage": "1",
      "varName": "applymsggdd",
      "name": "Clear reactions from message"
    },
    {
      "channel": "5",
      "varName": "channel",
      "message": "<:schreiben:760640649203941377> **|** Wie heißt du?",
      "storage": "1",
      "varName2": "frage",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "3",
      "varName": "channel",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "960000",
      "iftrue": "0",
      "iftrueVal": "24",
      "iffalse": "2",
      "iffalseVal": "60",
      "storage2": "1",
      "varName2": "a.name",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "frage",
      "message": "<:schreiben:760640649203941377> **|** Wie alt Bist du?",
      "storage2": "1",
      "varName2": "",
      "name": "Edit Message"
    },
    {
      "storage": "3",
      "varName": "channel",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "960000",
      "iftrue": "0",
      "iftrueVal": "2",
      "iffalse": "2",
      "iffalseVal": "60",
      "storage2": "1",
      "varName2": "a.alter",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "frage",
      "message": "<:schreiben:760640649203941377> **|** Erzähl Etwas über dich!",
      "storage2": "1",
      "varName2": "",
      "name": "Edit Message"
    },
    {
      "storage": "3",
      "varName": "channel",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "960000",
      "iftrue": "0",
      "iftrueVal": "2",
      "iffalse": "2",
      "iffalseVal": "60",
      "storage2": "1",
      "varName2": "a.erzähl",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "frage",
      "message": "<:schreiben:760640649203941377> **|** Was sind deine Erfahrungen / Referenzen?",
      "storage2": "1",
      "varName2": "",
      "name": "Edit Message"
    },
    {
      "storage": "3",
      "varName": "channel",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "960000",
      "iftrue": "0",
      "iftrueVal": "2",
      "iffalse": "2",
      "iffalseVal": "60",
      "storage2": "1",
      "varName2": "a.erfahr",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "frage",
      "message": "<:schreiben:760640649203941377> **|** Wie Erreichen wir dich? ( Discord / TS / Insta / Telegram / Signal )",
      "storage2": "1",
      "varName2": "",
      "name": "Edit Message"
    },
    {
      "storage": "3",
      "varName": "channel",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "960000",
      "iftrue": "0",
      "iftrueVal": "2",
      "iffalse": "2",
      "iffalseVal": "60",
      "storage2": "1",
      "varName2": "a.contact",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "frage",
      "message": "<:schreiben:760640649203941377> **|** Noch Weitere Infos / Anliegen? Schreib sie mir!",
      "storage2": "1",
      "varName2": "",
      "name": "Edit Message"
    },
    {
      "storage": "3",
      "varName": "channel",
      "filter": "content.length > 0 && author.id === user.id",
      "max": "1",
      "time": "960000",
      "iftrue": "0",
      "iftrueVal": "2",
      "iffalse": "2",
      "iffalseVal": "60",
      "storage2": "1",
      "varName2": "a.optional",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "frage",
      "message": "<:schreiben:760640649203941377> **|** Toll! Wir haben deine Bewerbung gesendet!",
      "storage2": "1",
      "varName2": "",
      "name": "Edit Message"
    },
    {
      "message": "1",
      "varName": "a.name",
      "info": "2",
      "storage": "1",
      "varName2": "f.name",
      "name": "Store Message Info"
    },
    {
      "message": "1",
      "varName": "a.alter",
      "info": "2",
      "storage": "1",
      "varName2": "f.alter",
      "name": "Store Message Info"
    },
    {
      "message": "1",
      "varName": "a.alter",
      "info": "2",
      "storage": "1",
      "varName2": "f.alter",
      "name": "Store Message Info"
    },
    {
      "message": "1",
      "varName": "a.erzähl",
      "info": "2",
      "storage": "1",
      "varName2": "f.erzähl",
      "name": "Store Message Info"
    },
    {
      "message": "1",
      "varName": "a.erfahr",
      "info": "2",
      "storage": "1",
      "varName2": "f.erfahr",
      "name": "Store Message Info"
    },
    {
      "message": "1",
      "varName": "a.contact",
      "info": "2",
      "storage": "1",
      "varName2": "f.contact",
      "name": "Store Message Info"
    },
    {
      "message": "1",
      "varName": "a.optional",
      "info": "2",
      "storage": "1",
      "varName2": "f.optional",
      "name": "Store Message Info"
    },
    {
      "storage": "1",
      "varName": "applymsggdd",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "a.name",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "a.alter",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "a.erzähl",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "a.erfahr",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "a.contact",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "storage": "1",
      "varName": "a.optional",
      "reason": "",
      "name": "Delete Message"
    },
    {
      "comment": "<strong>Channel ID Einsetzen</strong>",
      "color": "#ff0000",
      "name": "Comment"
    },
    {
      "info": "0",
      "find": "???",
      "storage": "1",
      "varName": "applychannel",
      "name": "Find Channel"
    },
    {
      "comment": "----------------------------------------",
      "color": "#ff0000",
      "name": "Comment"
    },
    {
      "title": "<:hakenja2:726933385787736085> Neue Bewerbung",
      "author": "",
      "color": "00ff00",
      "url": "",
      "authorIcon": "",
      "authorUrl": "",
      "imageUrl": "",
      "thumbUrl": "",
      "timestamp": "true",
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
      "fieldName": "Dein Name?",
      "message": "${tempVars(\"f.name\")}",
      "inline": "1",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "embed",
      "fieldName": "Dein Alter?",
      "message": "${tempVars(\"f.alter\")}",
      "inline": "1",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "embed",
      "fieldName": "Erzähl was über dich!",
      "message": "${tempVars(\"f.erzähl\")}",
      "inline": "1",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "embed",
      "fieldName": "Kontaktieren?",
      "message": "${tempVars(\"f.contact\")}",
      "inline": "1",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "embed",
      "fieldName": "Extra Infos",
      "message": "${tempVars(\"f.optional\")}",
      "inline": "1",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "embed",
      "message": "${tempVars(\"membererr\")}",
      "footerIcon": "",
      "name": "Set Embed Footer"
    },
    {
      "storage": "1",
      "varName": "embed",
      "channel": "5",
      "varName2": "applychannel",
      "storage3": "0",
      "varName3": "",
      "iffalse": "0",
      "iffalseVal": "",
      "messageContent": "",
      "name": "Send Embed Message"
    },
    {
      "time": "30",
      "measurement": "1",
      "name": "Wait"
    },
    {
      "storage": "3",
      "varName": "channel",
      "reason": "",
      "name": "Delete Channel"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "storage": "1",
      "varName": "frage",
      "message": "<:schreiben:760640649203941377> **|** Bewerbung Abgebrochen, Keine Antwort Erhalten!",
      "storage2": "1",
      "varName2": "",
      "name": "Edit Message"
    },
    {
      "time": "30",
      "measurement": "1",
      "name": "Wait"
    },
    {
      "storage": "3",
      "varName": "channel",
      "reason": "",
      "name": "Delete Channel"
    }
  ],
  "comType": "0"
}
```
