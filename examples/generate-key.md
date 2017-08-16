# Generate key (Player Protection)

Server-side code

```php
// serverside.php
$_projectId = 'project id';
$timestamp = new \DateTime('now');
$timestamp = $timestamp->getTimestamp();
$key = md5($_projectId.'vp7Hdb9rYRjcQqD'.$timestamp);
```

Embed player

```html
<h1>Video #1</h1>
<p>Some Text</p>
<!-- Player Container #1 -->
<div id="player1" style="width:100%;height:360px;"></div>
<script type="text/javascript" src="https://playout.3qsdn.com/player/js/sdnplayer.js"></script>
<script type="text/javascript"
        src="https://playout.3qsdn.com/7201c779-6b3c-11e7-a40e-002590c750be?js=true&
        timestamp=`timestamp`&key=`key`&container=player1&width=100%25&height=360
        &javaScriptBridgeFunction=myPlayerBridge">
</script>
```

Back to [index](../README.md).