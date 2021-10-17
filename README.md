# ChannelBox
ChannelBox it is a simple tool for Starlette framework that allows you send messages to named websocket channels.

Example of use:
- chats
- notifications from backend
- alerts 


```no-highlight
https://github.com/Sobolev5/channel-box
```

# Install
To install run:
```no-highlight
pip install channel-box
```

# [important] See full working example with websocket setup 
https://channel-box.andrey-sobolev.ru/channel/test/
https://github.com/Sobolev5/channel-box/tree/master/example

# [important] NGINX websocket setup
http://nginx.org/en/docs/http/websocket.html


# [important] Install uvicorn with websocket support
```no-highlight
pip install uvicorn[standard]
```

# channel_box methods

Send message to any group from any part of your code:
```no-highlight
await channel_box.channel_send("MySimpleChat", {"username": "another part code", "message": "hello from SendFromAnotherPartCode"}, show=True, history=True)
```

Show groups and channels:
```no-highlight
await channel_box.channels_show()  
```

Flush all groups and channels:
```no-highlight
await channel_box.channels_flush()
```

# Buy me a coffee [thanks]
https://www.buymeacoffee.com/AndreySobolev





