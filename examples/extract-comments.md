```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      .js3q-comment-list {
        flex-direction: column-reverse;
      }

      .js3q-comment-list js3q-sidebar-header {
        order: 1;
      }

      .js3q-comment-list js3q-sidebar-content {
        display: flex;
        flex-direction: column-reverse;
      }
    </style>
  </head>

  <body>
    <div id="player"></div>
    <div id="comments"></div>

    <script src="//player.3qsdn.com/js3q.latest.js"></script>

    <script>
      new js3q({
        container: 'player',
        dataid: 'your-data-id',
        comments: 'comments',
        comments_align: 'top',
      });
    </script>
  </body>
</html>
```
