# Fire-Ws-Client based by sockJs

Javascript client for [Fire WebSocket Server](https://github.com/dizard/FireWebSocketServer)

Include
```html
<script src="//cdn.jsdelivr.net/sockjs/0.3.4/sockjs.min.js"></script>
<script src="./fws.js"></script>
```

```javasript
var FWSClient = new FWS('host', 'nameSpace', 'authString);
FWSClient.on('auth', function(conId) {
    console.log('auth ok', conId);
    FWSClient.channel('@test', function(data) {
        console.log(data);
    });
});
```
