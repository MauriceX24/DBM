# Apply RawData
***
### Screenshots
![alt text](https://moon.is-inside.me/yRRWuXaW.png "Resultat")

![alt text](https://moon.is-inside.me/XM9uiWmc.png "Bewerbungsablauf")

![alt text](https://moon.is-inside.me/HmTDQIHm.png "Action #28 - Trage deine Channel ID ein!")

_Trage in **Action #28** deine Channel ID ein, um die Bewerbungen zu erhalten._
***
### RawData
```
{
  "name": "apply",
  "permissions": "NONE",
  "restriction": "1",
  "_id": "UDHJh",
  "actions": [
    {
      "channel": "0",
      "varName": "",
      "message": "**Herzlichen dank für deine Interesse!**\nBitte halte folgendes bereit:\n» Name\n» Alter\n» Dein fav. Spiel\n» Warum wir?\n\n_Reagiere auf ✅ um die Bewerbung zu starten._",
      "storage": "1",
      "varName2": "apply.greeting",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "1",
      "varName": "apply.greeting",
      "emoji": "4",
      "varName2": "✅",
      "varName3": "",
      "name": "Add Reaction"
    },
    {
      "member": "1",
      "varName": "",
      "info": "1",
      "storage": "1",
      "varName2": "UserID",
      "name": "Store Member Info"
    },
    {
      "storage": "1",
      "varName": "apply.greeting",
      "filter": "reaction.emoji.name === '✅' && user.id === '${tempVars(\"UserID\")}'",
      "max": "1",
      "time": "60000",
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
      "comment": "» Name",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**Wie ist dein richtiger Name, ${member}?**",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.match('') && author.id === '${tempVars(\"UserID\")}'",
      "max": "1",
      "time": "60000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "33",
      "storage2": "1",
      "varName2": "apply.name.a",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "apply.name.a",
      "name": "Delete Message"
    },
    {
      "comment": "» Age",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**Wie alt bist du, ${member}?**",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.match('') && author.id === '${tempVars(\"UserID\")}'",
      "max": "1",
      "time": "60000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "33",
      "storage2": "1",
      "varName2": "apply.age.a",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "apply.age.a",
      "name": "Delete Message"
    },
    {
      "comment": "» Fav Game",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**Was ist dein meist gespieltes Spiel, ${member}?**",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.match('') && author.id === '${tempVars(\"UserID\")}'",
      "max": "1",
      "time": "60000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "33",
      "storage2": "1",
      "varName2": "apply.fg.a",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "apply.fg.a",
      "name": "Delete Message"
    },
    {
      "comment": "» Why are you choosing us",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**Wieso magst du uns unterstützen, ${member}?**",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    },
    {
      "storage": "0",
      "varName": "",
      "filter": "content.match('') && author.id === '${tempVars(\"UserID\")}'",
      "max": "1",
      "time": "70000",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "2",
      "iffalseVal": "33",
      "storage2": "1",
      "varName2": "apply.ww.a",
      "name": "Await Response Call Action"
    },
    {
      "storage": "1",
      "varName": "apply.ww.a",
      "name": "Delete Message"
    },
    {
      "comment": "» Sende Embed",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "member": "1",
      "varName": "",
      "info": "22",
      "storage": "1",
      "varName2": "usertag",
      "name": "Store Member Info"
    },
    {
      "title": "Bewerbung von ${tempVars(\"usertag\")}",
      "author": "",
      "color": "",
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
      "fieldName": "Name",
      "message": "${tempVars(\"apply.name.a\")}",
      "inline": "0",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "embed",
      "fieldName": "Alter",
      "message": "${tempVars(\"apply.age.a\")}",
      "inline": "0",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "embed",
      "fieldName": "Lieblingsspiel",
      "message": "${tempVars(\"apply.fg.a\")}",
      "inline": "1",
      "name": "Add Embed Field"
    },
    {
      "storage": "1",
      "varName": "embed",
      "fieldName": "Warum wir?",
      "message": "${tempVars(\"apply.ww.a\")}",
      "inline": "1",
      "name": "Add Embed Field"
    },
    {
      "info": "0",
      "find": "523552948341571594",
      "storage": "1",
      "varName": "channel.sendembeds",
      "name": "Find Channel"
    },
    {
      "storage": "1",
      "varName": "embed",
      "channel": "5",
      "varName2": "channel.sendembeds",
      "storage3": "0",
      "varName3": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Embed Message"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**Deine Bewerbung wurde abgeschickt!**",
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
      "comment": "» Timeouts",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "channel": "0",
      "varName": "",
      "message": "**Noch da, ${member}?**\nDie Bewerbung wurde abgebrochen, da du zu lange für deine Antwort benötigt hast.",
      "storage": "0",
      "varName2": "",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Send Message"
    }
  ]
}
```
