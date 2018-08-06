# Receive Events via JavaScript

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
<script type="text/javascript">
   var js3qVideoPlayer;
    (function () {
        var _js3qi = setInterval(function () {
            if (typeof js3q != 'undefined') {
                clearInterval(_js3qi);
                js3qVideoPlayer = new js3q({
                    'data-id': '5c3b0910-8850-11e7-9273-002590c750be',
                    'container': 'player1',
                    'jscallback' : 'myPlayerBridge' // Name your Bridge here
                });
                js3qVideoPlayer.init();
            }
        }, 10);
    })();
</script>
```

JavaScript

```javascript
<script type="text/javascript">
function myPlayerBridge(player, event, data) {
    console.log(event);
}
</script>
```

Back to [index](../README.md).