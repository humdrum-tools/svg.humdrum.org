---
permalink: /index.html
---

{% include_relative listeners.html %}
{% include_relative scripts-local.html %}

<h1> MIDI-to-SVG converter </h1>


<nobr>MIDI file URL: <input type="text" onkeyup="updateSvg()" id="url" value="/midi/twinkle.mid" style="width:500px;"></nobr>
<br/>Try `/midi/sousa-occidental-march.mid` or a URL to any Standard MIDI File.
<br/>
<br/>

<nobr>Scale: <input type="text" onkeyup="updateSvg()" class="option" id="scale" value="5" style="width:50px;"></nobr>
<nobr>AspectRatio: <input type="text" onkeyup="updateSvg()" class="option" id="aspectRatio" value="15" style="width:50px;"></nobr>
<nobr>Opacity: <input type="text" onkeyup="updateSvg()" class="option" id="opacity" value="1.0" style="width:50px;"></nobr>

<nobr>Dark mode: <input type="checkbox" onchange="updateSvg()" class="option" id="dark"></nobr>
<nobr>Staff lines: <input type="checkbox" onchange="updateSvg()" class="option" id="grandstaff"></nobr>
<nobr>Clefs: <input type="checkbox" onchange="updateSvg()" class="option" id="clefs"></nobr>
<nobr>Rounded: <input type="checkbox" onchange="updateSvg()" class="option" id="rounded"></nobr>
<nobr>Velocity: <input type="checkbox" onchange="updateSvg()" class="option" id="velocity"></nobr>
<nobr>Connector lines: <input type="checkbox" onchange="updateSvg()" class="option" id="connector"></nobr>
<nobr>Embed data: <input type="checkbox" onchange="updateSvg()" class="option" id="data"></nobr>


<div style="width:100%; overflow-x: auto; padding-top:50px" id="display-area"></div>

<div id="options"></div>


