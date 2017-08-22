# Custom action after video is completed

Embed library at head or before last body

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
<div id="hiddenBox" style="display:none;">
    <a href="#">Download PDF</a>
</div>
```

JavaScript

```javascript
<script type="text/javascript">
var timeLimit = 60; // Time after Action should be called
var player = document.getElementById('player1')
function myPLayerBridge(player, event, data) {
    if(player.getFullPlaybackTime() >= timeLimit) {
        document.getElementById('hiddenBox').setAttribute('style', 'display:block;');
    }
}
</script>
```

Back to [index](../README.md).