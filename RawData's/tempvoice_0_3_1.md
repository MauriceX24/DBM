__**TempVoice-Event**__

Es ist möglich, dass diese RawData nicht bei dir funktoniert. Ich weiß nicht warum, aber bei vielen bereitet sie Probleme auf!

![trailer](https://moon.is-inside.me/oZlZcaTK.gif)
----------------------------------
```
{
  "name": "TempVoicechat 0.3",
  "temp": "1",
  "event-type": "22",
  "_id": "HPZzT",
  "actions": [
    {
      "member": "2",
      "varName": "2",
      "info": "19",
      "storage": "1",
      "varName2": "Member VoiceChat",
      "name": "Store Member Info"
    },
    {
      "member": "2",
      "varName": "2",
      "info": "2",
      "storage": "1",
      "varName2": "Member.Username",
      "name": "Store Member Info"
    },
    {
      "member": "2",
      "varName": "2",
      "info": "1",
      "storage": "1",
      "varName2": "Member.ID",
      "name": "Store Member Info"
    },
    {
      "channel": "3",
      "varName": "Member VoiceChat",
      "info": "2",
      "storage": "1",
      "varName2": "VoiceChat.name",
      "name": "Store Voice Channel Info"
    },
    {
      "storage": "1",
      "varName": "VoiceChat.name",
      "comparison": "1",
      "value": "Create Voice Chat",
      "iftrue": "3",
      "iftrueVal": "2",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Check Variable"
    },
    {
      "comment": "███ ↑ Setze deinen Channelname ↑",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "storage": "1",
      "varName": "VoiceChat.name",
      "comparison": "1",
      "value": "tempVars(\"Member.Username\")",
      "iftrue": "1",
      "iftrueVal": "18",
      "iffalse": "2",
      "iffalseVal": "24",
      "name": "Check Variable"
    },
    {
      "member": "2",
      "varName": "2",
      "dataName": "TV-ID",
      "defaultVal": "0",
      "storage": "1",
      "varName2": "TempVoice-MemData",
      "name": "Store Member Data"
    },
    {
      "info": "0",
      "find": "${tempVars(\"TempVoice-MemData\")}",
      "storage": "1",
      "varName": "TempVC.Exist?",
      "name": "Find Voice Channel"
    },
    {
      "storage": "1",
      "varName": "TempVC.Exist?",
      "comparison": "0",
      "value": "",
      "iftrue": "3",
      "iftrueVal": "8",
      "iffalse": "0",
      "iffalseVal": "",
      "name": "Check Variable"
    },
    {
      "comment": "███ Create Channel -------------------",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "channelName": "${tempVars(\"Member.Username\")}",
      "categoryID": "573489310175723520",
      "bitrate": "",
      "userLimit": "",
      "storage": "1",
      "varName": "VoiceChat-Member",
      "name": "Create Voice Channel"
    },
    {
      "channel": "3",
      "varName": "VoiceChat-Member",
      "info": "1",
      "storage": "1",
      "varName2": "TempChannel-ID",
      "name": "Store Voice Channel Info"
    },
    {
      "member": "2",
      "varName": "2",
      "dataName": "TV-ID",
      "changeType": "0",
      "value": "tempVars(\"TempChannel-ID\")",
      "name": "Control Member Data"
    },
    {
      "comment": "███ ↑ Setze deine Kategorie ↑",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "vchannel": "3",
      "varName": "VoiceChat-Member",
      "member": "2",
      "varName2": "2",
      "permission": "MANAGE_CHANNELS",
      "state": "0",
      "name": "Set Member Voice Channel Perms"
    },
    {
      "behavior": "0",
      "interpretation": "0",
      "code": "tempVars(\"2\").setVoiceChannel(tempVars(\"VoiceChat-Member\"));",
      "storage": "0",
      "varName": "",
      "name": "Run Script"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "member": "2",
      "varName": "2",
      "dataName": "TV-ID",
      "defaultVal": "0",
      "storage": "1",
      "varName2": "TempVoice.ChannelID",
      "name": "Store Member Data"
    },
    {
      "info": "0",
      "find": "${tempVars(\"TempVoice.ChannelID\")}",
      "storage": "1",
      "varName": "vvv",
      "name": "Find Voice Channel"
    },
    {
      "behavior": "0",
      "interpretation": "0",
      "code": "tempVars(\"2\").setVoiceChannel(tempVars(\"vvv\"));",
      "storage": "0",
      "varName": "",
      "name": "Run Script"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "comment": "███ Delete Channel ---------------------",
      "color": "#ffff00",
      "name": "Comment"
    },
    {
      "member": "2",
      "varName": "2",
      "dataName": "TV-ID",
      "defaultVal": "0",
      "storage": "1",
      "varName2": "TempVoice.ChannelID(Delete)",
      "name": "Store Member Data"
    },
    {
      "info": "0",
      "find": "${tempVars(\"TempVoice.ChannelID(Delete)\")}",
      "storage": "1",
      "varName": "TempVC.Delete",
      "name": "Find Voice Channel"
    },
    {
      "time": "30",
      "measurement": "1",
      "name": "Wait"
    },
    {
      "storage": "3",
      "varName": "TempVC.Delete",
      "name": "Delete Channel"
    },
    {
      "member": "2",
      "varName": "2",
      "dataName": "TV-ID",
      "changeType": "0",
      "value": "0",
      "name": "Control Member Data"
    }
  ],
  "temp2": "2"
}
```
