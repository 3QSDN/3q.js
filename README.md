# 3q.js Player documentation

Player documentation and embedding examples from [3Q SDN](https://www.3qsdn.com).

**General embedding**

Integrate Library at `<head>` or before last `</body>`
```html
<script type="text/javascript" async src="https://playout.3qsdn.com/player/js/sdnplayer.js"></script>
```

Place player container
```html
<div id="player1"></div>
```

Javascript (async)
```javascript
<script type="text/javascript">
   var js3qVideoPlayer;
    (function () {
        var _js3qi = setInterval(function () {
            if (typeof js3q != 'undefined') {
                clearInterval(_js3qi);
                js3qVideoPlayer = new js3q({
                    'data-id': '5c3b0910-8850-11e7-9273-002590c750be',
                    'container': 'player1',
                    'sticky': true,
                    'playlistbar' : true
                });
                js3qVideoPlayer.init();
            }
        }, 10);
    })();
</script>
```

* ### About
    * [HTML5 Video Player 3q.js](https://www.3qsdn.com/en/adaptive_html5_video_player).

* ### Examples
    * [Control player with javascript](examples/javascript-control-player.md)
    * [Receive Events](examples/receive-events.md)
    * [Custom action after video completed](examples/action-after-video-completed.md)
    * [Action when given time is reached](examples/action-after-given-time-is-reached.md)
    * [Embed Protected Player](examples/generate-key.md)

* ### Control
    * [Methods](docs/methods.md)
    * [Events](docs/events.md)

* ### Known Issues
    * [Cast Support](docs/cast-support.md)
    * [Using Require.js](docs/require-js.md)

* ### Configuration parameters
    * [List of parameters](docs/configuratoin-params.md)
