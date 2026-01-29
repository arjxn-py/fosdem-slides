<section>
  <h2 style="text-align:center; margin-top: 0.5rem; font-weight:300;">
    The current GIS model
  </h2>

  <p style="text-align:center; font-size:2.0rem; margin-top:1rem;">
    Many geospatial workflows still assume a
    <strong>desktop</strong>,
    <strong>local</strong>,
    <strong>single-user</strong> environment.
  </p>

  <div style="display:flex; justify-content:center; gap:4rem; align-items:center; margin-top:2.5rem;">
    <div style="text-align:center;">
      <img src="images/arcgis.png" alt="ArcGIS logo" style="height:15rem; display:block; margin:0 auto;" />
    </div>

  <div style="text-align:center;">
    <img src="images/qgis-logo.svg" alt="QGIS logo" style="height:15rem; display:block; margin:0 auto;" />
  </div>
  </div>

  <aside class="notes">
    This model works very well for individual analysis and professional desktop GIS.
    But it assumes a local machine, a single user, and a file-based workflow.
  </aside>
</section>


<section>

  <h3 style="text-align:center; margin-top:1.5rem;">
    GIS lives on a local machine
  </h3>

  <div style="display:flex; justify-content:center; gap:3rem; margin-top:2rem;">
    <img src="images/qgis-size.png" alt="QGIS install size" style="height:10rem;" />
  </div>

  <p style="text-align:center; margin-top:1rem;">
    Users install and manage the full stack locally.
  </p>
</section>


<section>

  <h3 style="text-align:center; margin-top:1.5rem;">
    Driven through rich desktop interfaces
  </h3>

  <div style="position:relative; height:70vh; margin-top:2rem;">
    <img src="images/qgis-ui.png" style="width:70%; border-radius:8px;" />
  </div>

  <aside class="notes">
    The interface is optimized for a single expert user working interactively.
  </aside>
</section>


<section>

  <h3 style="text-align:center; margin-top:0rem;">
    Files are the unit of collaboration
  </h3>

  <div style="display:flex; align-items:center; gap:3rem; max-width:80%; margin:0 auto;">
    <img src="images/teamwork.jpg" style="height:16rem;" />

  <!-- Text block -->
  <ul style="flex:1; list-style-type:disc; padding-left:1.5rem; margin:0; font-size:1.3rem; line-height:1.8; text-align:left;">
    <li>Files shared via Email, Git or Drives</li>
    <li>Difficult to Iterate</li>
    <li>Friction with multiperson tasks</li>
  </ul>

  </div>

</section>


<section>

  <h3 style="text-align:center; margin-top:1.5rem;">
    Visualization and computation are separate tools
  </h3>

  <div style="display:flex; align-items:center; justify-content:center; gap:3rem; height:70%;">
    <div style="flex:1; text-align:center;">
      <img src="images/qgis-vis.png" style="max-height:50vh;" />
      <p>Desktop GIS</p>
    </div>

  <!-- Switching Icon -->
  <div style="font-size:3rem;">🔄</div>

  <!-- Jupyter Screenshot -->
  <div style="flex:1; text-align:center;">
    <img src="images/jgis-ww.png" alt="Jupyter Screenshot"
          style="max-height:60vh; width:auto; border-radius:6px; box-shadow:0 4px 8px rgba(0,0,0,0.2);" />
    <p style="margin-top:0.5rem;">Jupyter for Processing</p>
  </div>

  </div>
  </div>

  <aside class="notes">
    Users switch between environments to visualize and compute.
  </aside>
</section>

