# Embed Protected Player

Server-side code

```php
// serverside.php

$_projectId = 'project id';
$_accountSecret = 'account_secret';
$timestamp = new \DateTime('now');
$timestamp = $timestamp->getTimestamp();
// You'll find the Project Key at Project Settings.
$key = md5($_projectId.$project_key.$timestamp);
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