# Events

player events can handled over javascript e.g.:

```javascript
function playerBridge(player,event,data) {
    switch(event) {
        case default:
            console.log(event+': '+data);
        break;
    }
}
```

<table width="100%">
<thead>
<tr>
<th>Event</th>
<th></th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
    <td>onJavaScriptBridgeCreated</td>
    <td></td>
    <td>bridge is ready</td>
</tr>
<tr>
    <td>ready</td>
    <td></td>
    <td>video is ready</td>
</tr>
<tr>
    <td>playing</td>
    <td></td>
    <td>video is playing</td>
</tr>
<tr>
    <td>paused</td>
    <td></td>
    <td>video is paused</td>
</tr>
<tr>
    <td>complete</td>
    <td></td>
    <td>video completed</td>
</tr>
<tr>
    <td>volumeChange</td>
    <td></td>
    <td>volume changed</td>
</tr>
<tr>
    <td>timeChange</td>
    <td></td>
    <td>current position changes</td>
</tr>
<tr>
    <td>durationChange</td>
    <td></td>
    <td>length of video changes</td>
</tr>
<tr>
    <td>errorEvent</td>
    <td></td>
    <td></td>
</tr>
<tr>
    <td>fullscreenChange</td>
    <td></td>
    <td>fullscreen state change</td>
</tr>
<tr>
    <td>crontrolbarChange</td>
    <td></td>
    <td>controlbar hides or shows/td>
</tr>
<tr>
    <td>advertisementStart</td>
    <td></td>
    <td>player starts requesting ads</td>
</tr>
<tr>
    <td>advertisementStop</td>
    <td></td>
    <td>adsrequest finished</td>
</tr>
<tr>
    <td>playRequest</td>
    <td></td>
    <td>user requested to play</td>
</tr>
<tr>
    <td>pauseRequest</td>
    <td></td>
    <td>user requested to pause</td>
</tr>
<tr>
    <td>seekRequest</td>
    <td></td>
    <td>user requested to seek to a specific position</td>
</tr>
<tr>
    <td>muted</td>
    <td></td>
    <td>video muted</td>
</tr>
<tr>
    <td>unmuted</td>
    <td></td>
    <td>video unmuted</td>
</tr>
</tbody>
</table>

Back to [index](../README.md).