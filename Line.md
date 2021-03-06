# Line 

## Incoming

For the incoming messages, Line provides the format with 3 different sources and 7 differnt event types.

- [Source](#source)
    - [user](#user-source)
    - [room](#room-source)
    - [group](#group-source)
- [Event Type](#event-type)
    - [Message](#message-event)
        - [Text](#text-message)
        - [Image](#image-message)
        - [Audio](#audio-message)
        - [File](#file-message)
        - [Location](#location-message)
        - [Sticker](#sticker-message)
    - [Follow](#follow-event)
    - [Unfollow](#unfollow-event)
    - [Join](#join-event)
    - [Leave](#leave-event)
    - [Postback](#postback-event)
    - [Beacon](#beacon-event)

### Source

- [user](#user-source)
- [room](#room-source)
- [group](#group-source)

#### User Source
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"text",
            "text":"Hello, world"
         }
      }
   ]
}
```

#### Room Source
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{
            "type": "room",
            "roomId": "Ra8dbf4673c4c812cd491258042226c99",
            "userId": "U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"text",
            "text":"Hello, world"
         }
      }
   ]
}
```

#### Group Source
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{
            "type": "group",
            "groupId": "Ca56f94637cc4347f90a25382909b24b9",
            "userId": "U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"text",
            "text":"Hello, world"
         }
      }
   ]
}
```


### Event Type

- [Message](#message-event)
- [Follow](#follow-event)
- [Unfollow](#unfollow-event)
- [Join](#join-event)
- [Leave](#leave-event)
- [Postback](#postback-event)
- [Beacon](#beacon-event)

#### Message Event

Message event type is most common event type people deal with. It can further divided into 7 types.

- [Text](#text-message)
- [Image](#image-message)
- [Audio](#audio-message)
- [File](#file-message)
- [Location](#location-message)
- [Sticker](#sticker-message)

##### Text Message
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"text",
            "text":"Hello, world"
         }
      }
   ]
}
```

##### Image Message
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"image"
         }
      }
   ]
}

```

##### Video Message
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"video"
         }
      }
   ]
}

```

##### Audio Message
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"audio"
         }
      }
   ]
}
```

##### File Message
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"file",
            "fileName":"file.txt",
            "fileSize":2138
         }
      }
   ]
}
```

##### Location Message
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"location",
            "title":"my location",
            "address":"〒150-0002 東京都渋谷区渋谷２丁目２１−１",
            "latitude":35.65910807942215,
            "longitude":139.70372892916203
         }
      }
   ]
}
```

##### Sticker Message
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"message",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "message":{  
            "id":"325708",
            "type":"sticker",
            "packageId":"1",
            "stickerId":"1"
         }
      }
   ]
}
```

#### Follow Event
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"follow",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         }
      }
   ]
}
```

#### Unfollow Event
```json
{  
   "events":[  
      {  
         "type":"unfollow",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         }
      }
   ]
}
```

#### Join Event
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"join",
         "timestamp":1462629479859,
         "source":{  
            "type":"group",
            "groupId":"cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         }
      }
   ]
}
```

#### Leave Event
```json
{  
   "events":[  
      {  
         "type":"leave",
         "timestamp":1462629479859,
         "source":{  
            "type":"group",
            "groupId":"cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         }
      }
   ]
}
```

#### Postback Event
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"postback",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "postback":{  
            "data":"action=buyItem&itemId=123123&color=red"
         }
      }
   ]
}
```

#### Beacon Event
```json
{  
   "events":[  
      {  
         "replyToken":"nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
         "type":"beacon",
         "timestamp":1462629479859,
         "source":{  
            "type":"user",
            "userId":"U206d25c2ea6bd87c17655609a1c37cb8"
         },
         "beacon":{  
            "hwid":"d41d8cd98f",
            "type":"enter"
         }
      }
   ]
}
```
