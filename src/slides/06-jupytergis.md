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


<section>
  <h2 style="text-align:center; margin-top:0.5rem;">
    How JupyterGIS Works
  </h2>

  <div style="display:flex; justify-content:center; align-items:flex-start; gap:2rem; flex-wrap:wrap; margin-top:2rem;">
    <!-- Rendering -->
    <div style="flex:1; min-width:220px; text-align:center;">
      <img src="images/openlayers.png" alt="Rendering" style="max-width:8rem; margin-bottom:0.5rem;" />
      <h3>Rendering</h3>
      <p>OpenLayers in-browser: vector & raster, dynamic styling</p>
    </div>

  <!-- Analysis -->
  <div style="flex:1; min-width:220px; text-align:center;">
    <img src="images/gdal.svg" alt="Analysis" style="max-width:8rem; margin-bottom:0.5rem;" />
    <h3>Analysis</h3>
    <p>GDAL compiled to WebAssembly - buffer, dissolve, rasterization, etc.</p>
  </div>

  <!-- Collaboration -->
  <div style="flex:1; min-width:220px; text-align:center;">
    <img src="images/collaboration-icon.png" alt="Collaboration" style="max-width:8rem; margin-bottom:0.5rem;" />
    <h3>Collaboration</h3>
    <p>Y.js CRDTs - live multi-user editing, conflict-free synchronization</p>
  </div>
  </div>

  <aside class="notes">
    Explain how these three components work together, and the .jgis file is the shared source of truth enabling fully interactive, collaborative GIS.
  </aside>
</section>
