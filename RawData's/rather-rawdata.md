# RRRather API
***
### How does look?
![alt text](https://moon.is-inside.me/PAwJkxPt.png "Screenshot")
***
### RawData
```
{
  "name": "rather",
  "permissions": "NONE",
  "restriction": "1",
  "_id": "DNIrg",
  "actions": [
    {
      "token": "",
      "user": "",
      "pass": "",
      "url": "https://www.rrrather.com/botapi",
      "path": "title",
      "storage": "1",
      "varName": "title",
      "debugMode": "1",
      "headers": "",
      "name": "Store Json From WebAPI"
    },
    {
      "token": "",
      "user": "",
      "pass": "",
      "url": "https://www.rrrather.com/botapi",
      "path": "choicea",
      "storage": "1",
      "varName": "answear.a",
      "debugMode": "1",
      "headers": "",
      "name": "Store Json From WebAPI"
    },
    {
      "token": "",
      "user": "",
      "pass": "",
      "url": "https://www.rrrather.com/botapi",
      "path": "choiceb",
      "storage": "1",
      "varName": "answear.b",
      "debugMode": "1",
      "headers": "",
      "name": "Store Json From WebAPI"
    },
    {
      "title": "${tempVars(\"title\")}",
      "author": "",
      "color": "#FFFFFF",
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
      "message": "**Choice A**\n${tempVars(\"answear.a\")}\n\n**Choice B**\n${tempVars(\"answear.b\")}",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "embed",
      "message": "Request to rrrather.com",
      "footerIcon": "",
      "name": "Set Embed Footer"
    },
    {
      "storage": "1",
      "varName": "embed",
      "channel": "0",
      "varName2": "",
      "storage3": "0",
      "varName3": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Embed Message"
    }
  ]
}
```
