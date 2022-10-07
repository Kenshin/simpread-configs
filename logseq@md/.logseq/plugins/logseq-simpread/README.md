<p align="center">
<p><img src="https://raw.githubusercontent.com/OverflowCat/logseq-simpread/master/logo/logo.svg" height="250px" width="250px"><br />
<large><b>logseq-simpread</b></large></p>
<p align="center">
<p>The official <a href="https://github.com/logseq/logseq">Logseq</a>
plugin of
<a href="https://github.com/Kenshin/simpread">SimpRead</a>.</p>
</p>
</p>
<p>https://user-images.githubusercontent.com/20166026/179386714-38d2c5e0-690f-4df4-82b3-d16108350fc1.mp4</p>
<h2 id="usage">Usage</h2>
<p>注意：本页面不包含使用教程，请前往简悦的 <a
href="https://github.com/Kenshin/simpread/discussions/4220">这条
discussion</a> 查看。</p>
<p>Currently the plugin contains only one function: triggering the
reading list panel.</p>
<p>To use this plugin, you need:</p>
<ul class="incremental">
<li>SimpRead, the browser extension installed</li>
<li>A premium account of SimpRead activated</li>
<li>Official <strong>简悦 · 同步助手</strong> installed, version &gt;=
1.1.0</li>
<li><strong>Knowledge base</strong> configured</li>
<li><strong>Automation</strong> configured and enabled</li>
<li><strong>Markdown 模板辅助增强插件</strong> installed and template
configured</li>
</ul>
<p>The template used in the demo video is under
<code>templates</code>.</p>
<h2 id="publishing">Publishing</h2>
<h3 id="packaging">Packaging</h3>
<p>The code is written in a single vanilla HTML file. The only
dependency is <code>lsplugin.user.min.js</code>. Just replace the one
loaded from CDN with a local copy.</p>
<h3 id="logo">Logo</h3>
<p>Note that some objects are hidden. You can <a
href="https://support.microsoft.com/en-us/office/manage-objects-with-the-selection-pane-a6b2fd3e-d769-46c1-9b9c-b94e04a72550">mamage
them with the Selection pane</a>.</p>
<p>To replicate <code>logo.svg</code>, please follow the instructions
below:</p>
<ol class="incremental">
<li>Open the XML file with PowerPoint</li>
<li>Select all elements in the slide (<kbd>Ctrl</kbd>+<kbd>A</kbd>)</li>
<li>Group them (<kbd>Ctrl</kbd>+<kbd>G</kbd>)</li>
<li>Paste the combination in SVG format
(<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>V</kbd>)</li>
<li>Right click, and save that SVG as a picture</li>
</ol>
<h2 id="known-issues">Known issues</h2>
<h3 id="top.document"><code>top.document</code></h3>
<p><code>top.document</code> may be removed by Logseq.</p>
<h3 id="color-of-the-toolbar-icon-looks-bad-in-some-themes">Color of the
toolbar icon looks bad in some themes</h3>
<p>Currently the toolbar icon is in SVG format, which requires
<code>.st1{stroke: #xxxxxx}</code> to control its color. However, most
buttons on the toolbar is in icon fonts, making unofficial themes like
Bear use another approach to control icon colors.</p>
<h3 id="scroll-bar">Scroll bar</h3>
<p>The style of the scroll bar of the iframe does not match the official
one’s.</p>
<h3 id="hardcoded-url">Hardcoded URL</h3>
<p>The port of simpread-sync is hardcoded to <code>7026</code>. A
configuration UI will be added in the future.</p>
<h2 id="roadmap">Roadmap</h2>
<p>A new plugin API based highlights synchronization will be added in
the future. Since Logseq plugins has no access to Node environment, it
is impossible to implement the API in the same way as using Local REST
API in Obsidian.</p>
