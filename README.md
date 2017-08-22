# 3q.js Player Doc

Player documentation and embedding examples from [3Q SDN](https://www.3qsdn.com).

* ### About
    * [HTML5 Video Player 3q.js](https://www.3qsdn.com/en/adaptive_html5_video_player).

* ### Examples
    * [Control player with javascript](examples/javascript-control-player.md)
    * [Receive Events](examples/receive-events.md)
    * [Custom action after video completed](examples/action-after-video-completed.md)
    * [Action when given time is reached](examples/action-after-given-time-is-reached.md)
    * [Embed Protected Player](examples/generate-key.md)

* ### Control
    * [Methods](docs/methods.md)
    * [Events](docs/events.md)

* ### Configuration parameters
    * [How to override](examples/player-configuration.md)

    The Player selects the configured settings, this parameters below can be overwritten.

    <table width="100%">
    <tr>
        <td>autoplay</td>
        <td>true | false</td>
        <td></td>
    </tr>
    <tr>
        <td>muted</td>
        <td>true | false</td>
        <td></td>
    </tr>
    <tr>
        <td>vast</td>
        <td>true | false</td>
        <td>Enables or disables configured ads in `AdManager`</td>
    </tr>
    <tr>
        <td>width</td>
        <td>100%25 | 640px</td>
        <td></td>
    </tr>
     <tr>
        <td>height</td>
        <td>100%25 | 360px</td>
        <td></td>
    </tr>
    <tr>
        <td>key</td>
        <td>string</td>
        <td></td>
    </tr>
    <tr>
        <td>timestamp</td>
        <td>string</td>
        <td></td>
    </tr>
    <tr>
        <td>controlbar</td>
        <td>true | false</td>
        <td>Enable or disable controls</td>
    </tr>
    <tr>
        <td>bgcolor</td>
        <td>#00000</td>
        <td>Background color video stage</td>
    </tr>
    <tr>
        <td>start</td>
        <td>30</td>
        <td>Generates an virutal subclip of the video</td>
    </tr>
    <tr>
        <td>end</td>
        <td>70</td>
        <td>Generates an virtual subclip of the video</td>
    </tr>
    </table>