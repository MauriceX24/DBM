# Global-Chat
--------------------
### Dieses System besteht aus einem
### [Event](https://github.com/MauriceX24/DBM/blob/master/RawData's/Global-Chat.md#event-1 "Klick zum Event") 
### und einem 
### [Command](https://github.com/MauriceX24/DBM/blob/master/RawData's/Global-Chat.md#command-1 "Klick zum Command")

## Screenshots
![image1](https://moon.is-inside.me/I95J5UDd.png "Erstelle deinen Chat-Namen")
![image2](https://moon.is-inside.me/nw9zQiYM.png "Ta-daaa > Global Chat")
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
      "channel": "0",
      "varName": "",
      "info": "2",
      "storage": "1",
      "varName2": "gc.name",
      "name": "Store Channel Info"
    },
    {
      "comment": "▼ ▼ ▼ Channelname (z.B 'global-chat')",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "storage": "1",
      "varName": "gc.name",
      "comparison": "1",
      "value": "'family'",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "1",
      "iffalseVal": "",
      "name": "Check Variable"
    },
    {
      "comment": "===========================",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "member": "1",
      "varName": "",
      "info": "0",
      "varName2": "",
      "iftrue": "1",
      "iftrueVal": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Check If Member"
    },
    {
      "message": "0",
      "varName": "",
      "info": "2",
      "storage": "3",
      "varName2": "gc.message",
      "name": "Store Message Info"
    },
    {
      "message": "0",
      "varName": "",
      "info": "3",
      "storage": "1",
      "varName2": "gc.author",
      "name": "Store Message Info"
    },
    {
      "member": "2",
      "varName": "gc.author",
      "info": "22",
      "storage": "3",
      "varName2": "Member.Tag",
      "name": "Store Member Info"
    },
    {
      "member": "2",
      "varName": "gc.author",
      "info": "16",
      "storage": "3",
      "varName2": "Member.Pic",
      "name": "Store Member Info"
    },
    {
      "server": "0",
      "varName": "",
      "info": "2",
      "storage": "3",
      "varName2": "gc.server.name",
      "name": "Store Server Info"
    },
    {
      "storage": "3",
      "varName": "gc.message",
      "comparison": "5",
      "value": "'discord.gg'",
      "iftrue": "3",
      "iftrueVal": "3",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Check Variable"
    },
    {
      "source": "eSegl",
      "list": "4",
      "varName": "",
      "tempVarName": "servers",
      "type": "true",
      "name": "Loop Through List"
    },
    {
      "storage": "0",
      "varName": "",
      "name": "Delete Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "channel": "0",
      "varName": "",
      "message": ":x: Keine Invites gestattet, ${member}!",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    }
  ],
  "comType": "3"
}
```
---------------------------
## Event
```
{
  "name": "<font color=\"orange\"> Global Chat </font>",
  "temp": "",
  "event-type": "0",
  "_id": "eSegl",
  "actions": [
    {
      "server": "1",
      "varName": "servers",
      "name": "Change Server"
    },
    {
      "info": "1",
      "find": "family",
      "storage": "1",
      "varName": "gc.server.channel",
      "name": "Find Channel"
    },
    {
      "title": "",
      "author": "${globalVars(\"Member.Tag\")}",
      "color": "",
      "url": "",
      "authorIcon": "${globalVars(\"Member.Pic\")}",
      "authorUrl": "",
      "imageUrl": "",
      "thumbUrl": "",
      "timestamp": "false",
      "text": "",
      "year": "",
      "month": "",
      "day": "",
      "hour": "",
      "minute": "",
      "second": "",
      "storage": "1",
      "varName": "gc.embed",
      "name": "Create Embed Message"
    },
    {
      "storage": "1",
      "varName": "gc.embed",
      "message": "${globalVars(\"gc.message\")}",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "gc.embed",
      "message": "Server - ${globalVars(\"gc.server.name\")}",
      "footerIcon": "",
      "name": "Set Embed Footer"
    },
    {
      "storage": "1",
      "varName": "gc.embed",
      "channel": "5",
      "varName2": "gc.server.channel",
      "storage3": "0",
      "varName3": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Embed Message"
    }
  ]
}
```
