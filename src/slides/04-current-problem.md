<section>
  <h2 style="text-align:center; margin-top: 0.5rem; font-weight:300;">
    How many of you are familiar with <strong style="font-weight:700;">FreeCAD</strong> or <strong style="font-weight:700;">QGIS</strong>?
  </h2>

  <div style="display:flex; justify-content:center; gap:4rem; align-items:center; margin-top:2.5rem;">
    <div class="fragment" style="text-align:center;">
      <img src="images/freecad-logo.svg" alt="FreeCAD logo" style="height:6rem; display:block; margin:0 auto;" />
    </div>

  <div class="fragment" style="text-align:center;">
    <img src="images/qgis-logo.svg" alt="QGIS logo" style="height:12rem; display:block; margin:0 auto;" />
  </div>
  </div>
</section>

<section>
  <h2 style="text-align:center; margin-top:0.5rem;">Powerful Tools BUT</h2>

  <div class="fragment" style="display:flex; flex-direction: column; align-items:center; gap:2rem; margin-top:2rem;">
  <h3 style="text-align:center; margin-top:1.5rem;">GB-sized installs</h3>

  <div style="text-align:center;">
    <img src="images/qgis-size.png" alt="QGIS install size" style="height:10rem; display:block; margin:0 auto;" />
  </div>
  <div style="text-align:center;">
    <img src="images/fcad-size.png" alt="FreeCAD install size" style="height:10rem; display:block; margin:0 auto;" />
  </div>
  </div>
</section>

<section>
  <h2 style="text-align:center; margin-top:0.5rem;">Powerful Tools BUT</h2>

  <div class="fragment" style="position:relative; height:80vh; margin-top:2rem;">

  <h3 style="position:absolute; top:1rem; width:100%; text-align:center;">Complex UI</h3>

  <div style="position:absolute; top:0; left:10%; width:60%; z-index:1;">
    <img src="images/qgis-ui.png" alt="QGIS UI screenshot" style="width:100%; height:auto; border-radius:8px; box-shadow:0 4px 8px rgba(0,0,0,0.2);" />
  </div>

  <div style="position:absolute; top:20%; left:30%; width:60%; z-index:2;">
    <img src="images/fcad-ui.png" alt="FreeCAD UI screenshot" style="width:100%; height:auto; border-radius:8px; box-shadow:0 4px 8px rgba(0,0,0,0.2);" />
  </div>
  </div>
</section>


<section>
  <h2 style="text-align:center; margin-top:0.5rem;">Powerful Tools BUT</h2>

  <div class="fragment" style="display:flex; flex-direction:column; justify-content:center; align-items:center; height:75vh; gap:2rem;">
    
  <h3 style="text-align:center; margin-top:2rem;">Not Collaborative</h3>

  <div style="display:flex; align-items:center; gap:3rem; max-width:80%;">
    
  <!-- Icon/illustration block -->
  <div style="flex:1; display:flex; justify-content:center; align-items:center;">
    <img src="images/teamwork.jpg" alt="Not collaborative" 
          style="max-height:70rem; width:auto; opacity:0.9;" />
  </div>

  <!-- Text block -->
  <ul style="flex:1; list-style-type:none; padding:0; margin:0; font-size:2.3rem; line-height:1.8; text-align:left;">
    <li>📧 Files shared via Email, Git or Drives</li>
    <li>🚫 Difficult to Iterate</li>
    <li>⚡ Friction with multiperson tasks</li>
  </ul>

  </div>

  </div>
</section>


<section>
  <h2 style="text-align:center; margin-top:0.5rem;">Powerful Tools BUT</h2>

  <div class="fragment" style="display:flex; flex-direction:column; align-items:center; height:75vh; gap:2rem;">
  
  <h3 style="text-align:center; margin:0;">Constant Context Switching</h3>

  <div style="display:flex; align-items:center; justify-content:center; gap:3rem; height:70%;">
    
  <!-- QGIS Screenshot -->
  <div style="flex:1; text-align:center;">
    <img src="images/qgis-vis.png" alt="QGIS Screenshot"
          style="max-height:60vh; width:auto; border-radius:6px; box-shadow:0 4px 8px rgba(0,0,0,0.2);" />
    <p style="margin-top:0.5rem;">QGIS for Visualization</p>
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

  <!-- Slide notes -->
  <aside class="notes">
    Here I want to emphasize the constant switching users face.  
    For example, you might analyze geospatial data in Jupyter, but as soon as you need visualization,  
    you jump to QGIS — then back again when you need further processing.  
    This breaks your flow, adds overhead, and makes reproducibility harder.
  </aside>
</section>

<section>
  <h2 style="text-align:center; margin-top:0.5rem;">Powerful Tools BUT</h2>

  <div class="fragment" style="position:relative; width:100%; height:70vh; margin-top:2rem; display:flex; flex-direction:column; align-items:center; justify-content:center;">
  <h3 style="margin-top:1.5rem; text-align:center;">Not Easily Shareable</h3>

  <div style="position:relative; width:100%; height:100%; display:flex; justify-content:center; align-items:center;">

  <img src="images/works-on-my-machine-ryan-gosling.png"
        alt="QGIS Error"
        style="max-width:70%; max-height:50%; border-radius:6px; margin-right:50%;" />

  <img src="images/qgis-versions.png"
        alt="QGIS Version Hell"
        style="position:absolute; bottom:5%; right:20%; max-height:85%; width:auto; border-radius:6px;" />

  </div>

  </div>
</section>
