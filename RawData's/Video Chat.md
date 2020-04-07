**VideoChat**

![Create](https://moon.is-inside.me/X7OvCzEP.png)

![Finish](https://moon.is-inside.me/yj0PN4WX.png)

![Result](https://moon.is-inside.me/AJEin3sI.png)
---------------------------------------- 
```
{
  "name": "video",
  "permissions": "NONE",
  "restriction": "1",
  "_id": "BauUP",
  "actions": [
    {
      "member": "1",
      "varName": "",
      "info": "4",
      "varName2": "",
      "iftrue": "3",
      "iftrueVal": "2",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Check If Member"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "Dies funktoniert nur, wenn du in einem Voice-Chat bist ${member}!",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "title": "Video Channel",
      "author": "",
      "color": "918FF0",
      "url": "",
      "authorIcon": "",
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
      "varName": "Embed1",
      "name": "Create Embed Message"
    },
    {
      "member": "1",
      "varName": "",
      "info": "19",
      "storage": "1",
      "varName2": "VoiceChannel",
      "name": "Store Member Info"
    },
    {
      "channel": "0",
      "varName": "",
      "info": "2",
      "storage": "1",
      "varName2": "VC Name",
      "name": "Store Voice Channel Info"
    },
    {
      "storage": "1",
      "varName": "Embed1",
      "message": "_Erstelle Video für `${tempVars(\"VC Name\")}`_",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "Embed1",
      "channel": "0",
      "varName2": "",
      "storage3": "1",
      "varName3": "Embed1.obj",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Embed Message"
    },
    {
      "time": "3",
      "measurement": "1",
      "name": "Wait"
    },
    {
      "channel": "0",
      "varName": "",
      "info": "1",
      "storage": "1",
      "varName2": "VCID",
      "name": "Store Voice Channel Info"
    },
    {
      "server": "0",
      "varName": "",
      "info": "1",
      "storage": "1",
      "varName2": "ServID",
      "name": "Store Server Info"
    },
    {
      "title": "Video Channel",
      "author": "",
      "color": "GREEN",
      "url": "",
      "authorIcon": "",
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
      "varName": "Embed2",
      "name": "Create Embed Message"
    },
    {
      "storage": "1",
      "varName": "Embed2",
      "message": "**Klicke [hier](https://discordapp.com/channels/${tempVars(\"ServID\")}/${tempVars(\"VCID\")}) um den Video-Chat beizutreten!**",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "Embed1.obj",
      "storage2": "1",
      "varName2": "Embed2",
      "name": "Edit Embed"
    }
  ]
}
```
