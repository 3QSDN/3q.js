# Methods

player methods can handled over javascript e.g.:

* ### Usage

```javascript
var js3qVideoPlayer;
    (function () {
       ... // player code here
    })();

js3qVideoPlayer.play(); // Calls method play
```

* ### List of methods

<table width="100%">
<thead>
<tr>
<th>Method</th>
<th></th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
    <td>play (play2 deprecated)</td>
    <td></td>
    <td>plays video</td>
</tr>
<tr>
    <td>pause</td>
    <td></td>
    <td>pauses video</td>
</tr>
<tr>
    <td>mute</td>
    <td></td>
    <td>mutes video</td>
</tr>
<tr>
    <td>unmute</td>
    <td></td>
    <td>unmutes video</td>
</tr>
<tr>
    <td>seek</td>
    <td>(int) seconds</td>
    <td>seeks to position</td>
</tr>
<tr>
    <td>getCurrentTime</td>
    <td>(int) seconds</td>
    <td>current position</td>
</tr>
<tr>
    <td>getDuration</td>
    <td>(int) seconds</td>
    <td>video length</td>
</tr>
<tr>
    <td>getVolume</td>
    <td>(int) 0.1 .. 1.0</td>
    <td>get volume</td>
</tr>
<tr>
    <td>setVolume</td>
    <td>(int) 0.1 .. 1.0</td>
    <td>get volume</td>
</tr>
<tr>
    <td>getSubtitles</td>
    <td>[Object]</td>
    <td>array of available subtitles</td>
</tr>
<tr>
    <td>setSubtitles</td>
    <td>(int) index</td>
    <td>set subtitle</td>
</tr>
<tr>
    <td>getAudioTracks</td>
    <td>[Object]</td>
    <td>array of available audiotracks</td>
</tr>
<tr>
    <td>setAudioTrack</td>
    <td>(int) index</td>
    <td>set audiotrack by index</td>
</tr>
<tr>
    <td>hideControlbar</td>
    <td></td>
    <td>hides player controls</td>
</tr>
<tr>
    <td>getLiveDelayInSeconds</td>
    <td>(int) seconds</td>
    <td>Live delay in seconds, not available on DVR</td>
</tr>
<tr>
    <td>getPlaybackTime</td>
    <td>(int) seconds</td>
    <td>get current viewing time (pageview)</td>
</tr>
<tr>
    <td>getFullPlaybackTime</td>
    <td>(int) seconds</td>
    <td>get full playback time (user and video)</td>
</tr>
<tr>
    <td>showSideBarInfoIcon</td>
    <td></td>
    <td>displays the sidebar info icon (top-right)</td>
</tr>
<tr>
    <td>showSideBar</td>
    <td></td>
    <td>displays the sidebar</td>
</tr>
<tr>
    <td>hideSideBar</td>
    <td></td>
    <td>hides the Sidebar</td>
</tr>
<tr>
    <td>setSideBarHTML</td>
    <td></td>
    <td>sets the HTML of the sidebar</td>
</tr>
<tr>
    <td>fullscreen</td>
    <td></td>
    <td></td>
</tr>
<tr>
    <td>exitfullscreen</td>
    <td></td>
    <td></td>
</tr>
</tbody>
</table>

Back to [index](../README.md).