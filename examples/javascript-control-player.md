# Control player with JavaScript

Embed library at head

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />

    <!-- Additional Headers -->

    <script src="//player.3qsdn.com/js3q.latest.js"></script>
  </head>
  <body>
    <!-- Additional Body Content -->

    <div id="player"></div>

    <button id="play">Play</button>
    <button id="pause">Pause</button>

    <script>
      // Initialize the player
      var js3qPlayer = new js3q({
        dataid: 'c3eaa1e0-c608-11ea-b206-0cc47a188158',
        container: 'player',
      })

      // Add the event handler for the 'Play' button
      var playBtn = document.getElementById('play')
      playBtn.addEventListener('click', function () {
        js3qPlayer.play()
      })

      // Add the event handler for the 'Pause' button
      var pauseBtn = document.getElementById('pause')
      pauseBtn.addEventListener('click', function () {
        js3qPlayer.pause()
      })
    </script>
  </body>
</html>
```

Back to [index](../README.md).
