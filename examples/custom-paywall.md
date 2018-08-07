# Custom Paywall when video completes

Embed library at head or before last body

```html
<script type="text/javascript" src="https://playout.3qsdn.com/player/js/sdnplayer.js"></script>
```

Embed player

```html
<h1>Video #1</h1>
<p>Some Text</p>
<!-- Player -->
<div id="player1" style="width:100%;height:360px;"></div>
<!-- Content which will be displayed at the end of the video -->
<div id="previewContent" style="display:none;">
        <p style="font-style:normal"><span class="icon-switch size24"></span>
        Starten Sie jetzt Ihre 14-tägige kostenlose Testphase!
        </p>
    <a class="btn-signup-content" href="https://sdn.3qsdn.com/de/register" target="_blank">Konto erstellen</a></div>
```

JavaScript

```javascript
<script type="text/javascript">
var js3qVideoPlayer;
    function sdnPlayerBridge(player,event,data) {
        switch (event) {
            case "complete":
                js3qVideoPlayer.showSideBarInfoIcon();
                js3qVideoPlayer.setSideBarHTML(document.getElementById('previewContent').innerHTML);
                js3qVideoPlayer.showSideBar();
                js3qVideoPlayer.hideControlbar();

            break;
        }
    }

    (function () {
        var _js3qi = setInterval(function () {
            if (typeof js3q != 'undefined') {
                clearInterval(_js3qi);
                js3qVideoPlayer = new js3q({
                    'data-id': '9293f091-c331-11e7-9273-002590c750be',
                    'container': 'player1',
                    'sticky': true,
                    'playlistbar' : true,
                    'layout' : 'responsive',
                    'end' : 15,
                    'jscallback': 'sdnPlayerBridge'
                });
                js3qVideoPlayer.init();
            }
        }, 10);
    })();
</script>
```

Back to [index](../README.md).