# Embed Protected Player

Server-side code

```php
// serverside.php

$_project_id = 'project id';
$_project_key = 'project_secret';
// You'll find the Project Key at Project Settings.

$timestamp = new \DateTime('now');
$timestamp = $timestamp->getTimestamp();


$key = md5($_project_id.$_project_key.$timestamp);
```

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
   var js3qVideoPlayer;
    (function () {
        var _js3qi = setInterval(function () {
            if (typeof js3q != 'undefined') {
                clearInterval(_js3qi);
                js3qVideoPlayer = new js3q({
                    'data-id': '5c3b0910-8850-11e7-9273-002590c750be',
                    'container': 'player1',
                    'sticky': true,
                    'key' : {key},
                    'timestamp' : {timestamp}
                });
                js3qVideoPlayer.init();
            }
        }, 10);
    })();
```

Back to [index](../README.md).