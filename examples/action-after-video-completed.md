# Custom action after video is completed

Embed library at head

```html
<script type="text/javascript" src="https://playout.3qsdn.com/player/js/sdnplayer.js"></script>
```

Embed player

```html
<h1>Video #1</h1>
<p>Some Text</p>
<!-- Player Container #1 -->
<div id="player1" style="width:100%;height:360px;"></div>
<script type="text/javascript" src="https://playout.3qsdn.com/7201c779-6b3c-11e7-a40e-002590c750be?js=true&container=player1&width=100%25&height=360&javaScriptBridgeFunction=myPlayerBridge">
</script>
```

JavaScript

```javascript
<script type="text/javascript">
function myPLayerBridge(player, event, data) {
    switch(event) {
        case "complete":
            // do something
        break;
    }
}
</script>
```

Back to [index](../README.md).