<section>
  <h2 style="text-transform: none;">
    JupyterGIS
    <img
      src="images/jgis.png"
      alt="JupyterGIS"
      style="height: 1em; vertical-align: middle; margin-right: 0.3em;"
    />
  </h2>
  <video
    src="video/jgis/jgis.mp4"
    autoplay
    loop
    muted
    playsinline
    style="max-width: 80%; margin-top: 2rem;"
  ></video>
</section>

<section>
  <h2 style="text-align:center; margin-top:0.5rem;">
    .jgis - The Live GIS Document
  </h2>

  <p style="text-align:center; font-size:1.6rem; margin-top:1rem;">
    A JSON-based representation of the entire GIS state
  </p>

  <div style="display:flex; justify-content:center; align-items:center; gap:3rem; margin-top:2rem; flex-wrap:wrap;">
    <!-- Left: bullets -->
    <ul style="flex:1; min-width:300px; font-size:1.4rem; line-height:1.8;">
      <li>Layers are live, editable objects</li>
      <li>Symbology updates instantly</li>
      <li>Analysis can run directly in the notebook</li>
      <li>Collaborative metadata ensures consistent multi-user state</li>
    </ul>

  <!-- Right: visual -->
  <div style="flex:1; min-width:300px; text-align:center;">
    <img src="images/jgis-venn.png"
        alt=".jgis document diagram"
        style="max-width:100%; border-radius:6px;" />
  </div>
  </div>

  <aside class="notes">
    Highlight that each layer is not a static file anymore, but a live object in the notebook. Everything happens interactively in the browser.
  </aside>
</section>
