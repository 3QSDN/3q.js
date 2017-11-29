# Muted Autoplay on mobile

```html
<script type="text/javascript" src="https://playout.3qsdn.com/player/js/sdnplayer.js"></script>
```

Embed player

```html
<h1>Video #1</h1>
<p>Some Text</p>
<!-- Player -->
<div id="player1" style="width:100%;height:360px;"></div>
```

JavaScript

```javascript
<script type="text/javascript">
var _autoplay = true;
var _muted = false;
var isMobilePlatform = function () {
        return (navigator.userAgent.match(/(iPod|iPhone|iPad)/) ||
        navigator.userAgent.toLowerCase().indexOf('android') > -1);
};

if(isMobilePlatform() == true) {
    _autoplay = true;
    _muted = true;
}

var js3qVideoPlayer;
    (function () {
        var _js3qi = setInterval(function () {
            if (typeof js3q != 'undefined') {
                clearInterval(_js3qi);
                js3qVideoPlayer = new js3q({
                    'data-id': '9293f091-c331-11e7-9273-002590c750be',
                    'container': 'player1',
                    'sticky': true,
                    'autoplay' : _autoplay,
                    'muted' : _muted,
                    'layout' : 'responsive'
                });
                js3qVideoPlayer.init();
            }
        }, 10);
    })();
</script>
```

Back to [index](../README.md).