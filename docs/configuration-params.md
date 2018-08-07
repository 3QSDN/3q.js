# Configuration Parameters

The Player selects the configured settings, this parameters below can be overwritten.

* ### List of parameters

<table width="100%">
<thead>
<tr>
<th>Parameter</th>
<th></th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>locale</td>
<td>string</td>
<td>en|de (more languages soon, Default is browser setting)</td>
</tr>
<tr>
<td>data-id</td>
<td>uuid</td>
<td>Known as sdnplayoutid or data-id; refers to video, playlist or live content</td>
</tr>
<tr>
<td>**sticky**</td>
<td>(bool) true|false</td>
<td>Pins video while scrolling</td>
</tr>
<tr>
<td>scrolltoplay</td>
<td>(bool) true|false</td>
<td>Only works when autoplay is disabled</td>
</tr>
<tr>
<td>autoplay</td>
<td>(bool) true|false</td>
<td></td>
</tr>
<tr>
<td>muted</td>
<td>(bool) true|false</td>
<td></td>
</tr>
<tr>
<td>vast</td>
<td>(bool) true|false</td>
<td>Enables or disables configured ads in `AdManager`</td>
</tr>
<tr>
<td>vastid</td>
<td>(int) id</td>
<td>Choose specific AdManager tag by id</td>
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
<td>(string)</td>
<td>*[Embed protected player](../examples/generate-key.md)</td>
</tr>
<tr>
<td>timestamp</td>
<td>(string)</td>
<td></td>
</tr>
<tr>
<td>controlbar</td>
<td>(bool) true | false</td>
<td>Enable or disable controls</td>
</tr>
<tr>
<td>controlbarautohide</td>
<td>(bool) true | false</td>
<td></td>
</tr>
<tr>
<td>bgcolor</td>
<td>(string) #00000</td>
<td>Background color video stage</td>
</tr>
<tr>
<td>start</td>
<td>(int) seconds</td>
<td>Start of virtual subclip</td>
</tr>
<tr>
<td>end</td>
<td>(int) seconds</td>
<td>End of virtual subclip</td>
</tr>
<tr>
<td>skin</td>
<td>(string)</td>
<td>Your custom Skin name</td>
</tr>
<tr>
<td>jscallback</td>
<td>(string)</td>
<td>Your global function for receiving events</td>
</tr>
</tbody>
</table>

* ### Parameters for comments

<table width="100%">
<thead>
<tr>
<th>Parameter</th>
<th></th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>firstname</td>
<td>(string)</td>
<td>Name for comments</td>
</tr>
<tr>
<td>surname</td>
<td>(string)</td>
<td>Name for comments</td>
</tr>
</tbody>
</table>

Back to [index](../README.md).