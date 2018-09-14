# 3q.js player documentation

Player documentation and embedding examples from [3Q](https://3q.video/en/developers).

## Table of contents

- [General Embedding](#general-embedding)
- [About](#about)
- [Control](#control)
- [Examples](#examples)
- [Known Issues](#known-issues)
- [Release Notes](#release-notes)

### General embedding

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
    * [HTML5 Video Player 3q.js](https://3q.video/en/adaptive_html5_video_player).
    * [Test Browser capabilities](https://3q.video/en/player-about-en).

* ### Configuration
    * [List of parameters](docs/configuration-params.md)

* ### Control
    * [Methods](docs/methods.md)
    * [Events](docs/events.md)

* ### Examples
    * [Control player with javascript](examples/javascript-control-player.md)
    * [Receive events](examples/receive-events.md)
    * [Custom action after video completed](examples/action-after-video-completed.md)
    * [Action when given time is reached](examples/action-after-given-time-is-reached.md)
    * [Embed protected player](examples/generate-key.md)

* ### Known Issues
    * [Cast Support](docs/cast-support.md)
    * [Using Require.js](docs/require-js.md)

### Release Notes

* #### 2018-09-14
    * Added custom GA function parameter
    
* #### 2018-08-07
    * Bugfix video looping if autoplay enabled and ads disabled

* #### 2018-07-27 (v4.1.1)
    * Added events: subtitleChange, audioChange
    * Added methods: getAudioTracks, setAudioTrack
    * Code clean up
    * Cast Support: Removed google's media library from code-base; Added subtitle and alternative audio support

* #### 2018-07-20
    * Improved handling on manifest load timeouts

* #### 2018-07-18
    * Sticky feature improvement
    * Fixed thumbnail aspect ratio on IE11

* #### 2018-07-11
    * Settings menu UI improvement for mobile
    * Improved handling for streams with alternative audio on ios and safari

* #### 2018-07-09 (v4.1.0)
    * getLiveDelayInSeconds() added for live streams
    * locale config param added

* #### 2018-06-20
    * Added new audio player UI including visualizer
    * Code clean up

* #### 2018-06-18
    * Added view port and env to debug info
    * Hide cast button while playing ads
    * Hide volume slider after muting/unmuting on mobile
    * Hide ads countdown when remaining time is not available by api
    * Improved ready callback
    * Added poster frame preload before displaying

* #### 2018-06-15
    * Fixed unrecognized jscallback Parameter (audio on-demand)
    * Added custom SkipButton UI for Google IMA

* #### 2018-06-14
    * Fixed player-ui issues on IE 10
    * Code clean up
    * Fixed player-ui issue regarding buffering spinner after postroll
    * Fixed missing ready call for audio streams



(c) 2009 - 2018 3Q GmbH, All rights reserved


