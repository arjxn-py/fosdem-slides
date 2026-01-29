<!-- .slide -->
<div style="text-align: left; line-height: 1.2; position: relative;">

  <h2 style="font-size: 1.6em; margin: 0; font-weight: 600;">
    JupyterGIS - Interactive, Collaborative, <br/>
    Client-Side GIS in JupyterLab
    <a href="https://jupytergis.readthedocs.io/en/latest/lite/lab/" target="_blank">
      <img src="images/jgis.png" alt="JupyterGIS" 
           style="height: 1em; vertical-align: middle; margin-left: 0.3em;" />
    </a>
  </h2>

  <p style="margin-top: 0.6em; font-size: 0.9em;">
    Arjun Verma · QuantStack
  </p>

  <div style="margin-top: 0.8em;">
    <img src="images/logo-qs.svg" alt="QuantStack" 
         style="height: 2.6em; vertical-align: middle;" />
    <img src="images/jupyter.svg" alt="Jupyter" 
         style="height: 2.6em; vertical-align: middle; margin-left: 0.6em;" />
    <img src="images/jupyterlite.png" alt="JupyterLite" 
         style="height: 2.6em; vertical-align: middle; margin-left: 0.3em;" />
  </div>

  <!-- QR Code -->
  <img src="images/slide-qr.svg" 
       alt="QR Code" 
       style="position: absolute; bottom: 1rem; right: 1rem; height: 13rem;" />
</div>
<!-- .slide: data-transition="zoom" -->


---

<!-- .slide: class="section-with-footer" -->

<!-- Heading -->
<!-- <div style="text-align: center; margin: 0.5rem 0 1rem;">
  <h2>About Us</h2>
</div>

<div style="display: flex; align-items: flex-start; justify-content: space-between; gap: 40px; font-size: 0.6em; line-height: 1.4;">

  <div style="flex: 1; min-width: 320px;">
    <div style="margin-bottom: 1.2em;">
      <strong style="font-size: 1.2em;">Arjun Verma</strong><br/>
      <span style="color: #666;">Scientific Software Developer</span><br/>
      <span style="color: #999; font-size: 0.9em;">QuantStack</span>
    </div>

  <div>
    <strong style="font-size: 1.2em;">Martin Renou</strong><br/>
    <span style="color: #666;">Technical Director</span><br/>
    <span style="color: #999; font-size: 0.9em;">QuantStack</span>
  </div>
  </div>

  <div style="flex: 1; text-align: center; min-width: 280px;">
    <div style="margin-top: 0.5em;">
      <img src="images/logo-qs.svg" alt="QuantStack Logo" style="height: 4em; max-width: 100%;" />
    </div>
  </div>

</div> -->


---

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



---

<section>
  <h2 style="text-align:center; font-size:2.6rem; margin-top:0.5rem;">
    Jupyter already changed how we work with data
  </h2>

  <p style="text-align:center; font-size:1.6rem; margin-top:1rem;">
    Notebooks are <strong>collaborative</strong>, <strong>reproducible</strong> computational documents.
  </p>

  <div style="display:flex; align-items:center; justify-content:center; gap:3rem; margin-top:2.5rem;">

<!-- Left: bullets -->
<ul style="flex:1; list-style-type:disc; font-size:1.4rem; line-height:1.8;">
    <li>Code, data, outputs, and narrative in one place</li>
    <li>Shareable, reproducible workflows</li>
    <li>Real-time collaboration</li>
    <li>Runs on desktop and in the browser</li>
</ul>

<!-- Right: visual -->
<div style="flex:1; text-align:center;">
    <img src="images/jupyterlab-screenshot.webp"
        alt="JupyterLab notebook"
        style="max-height:22rem; border-radius:8px; box-shadow:0 4px 12px rgba(0,0,0,0.2);" />
    <p style="font-size:1rem; margin-top:0.5rem;">
    Code • Output • Markdown • Collaboration
    </p>
</div>

  </div>

  <aside class="notes">
    In Jupyter, we already treat computation as a narrative.
    Everything is live, reproducible, and increasingly collaborative.
  </aside>
</section>


---

<section style="position:relative; height:80vh;">
  <h2 style="text-align:center; margin-top:0.5rem;">What IF?</h2>

  <div style="position:relative; width:100%; height:100%; margin-top:2rem; display:flex; flex-wrap:wrap; justify-content:space-around; align-items:flex-start; gap:2rem; padding:2rem;">
    <div style="flex:0 1 40%; font-weight:400; background:#f0f0f0; padding:0.5rem 1rem; border-radius:6px;">
      ✅ Very small to no install
    </div>
    <div style="flex:0 1 40%; font-weight:400; background:#f0f0f0; padding:0.5rem 1rem; border-radius:6px;">
      ✅ Non-overwhelming, beginner-friendly UI
    </div>
    <div style="flex:0 1 40%; font-weight:400; background:#f0f0f0; padding:0.5rem 1rem; border-radius:6px;">
      ✅ With live collaboration support
    </div>
    <div style="flex:0 1 40%; font-weight:400; background:#f0f0f0; padding:0.5rem 1rem; border-radius:6px;">
      ✅ Inside your notebooks & scientific environment
    </div>
    <div style="flex:0 1 40%; font-weight:400; background:#f0f0f0; padding:0.5rem 1rem; border-radius:6px;">
      ✅ Interoperable across tools & formats
    </div>
    <div style="flex:0 1 40%; font-weight:400; background:#f0f0f0; padding:0.5rem 1rem; border-radius:6px;">
      ✅ Highly extensible
    </div>
  </div>
</section>

<section style="display:flex; justify-content:center; align-items:center; height:100vh; flex-direction:column; gap:2rem;">
  <h2 style="margin:0; text-align:center;">
    JupyterCAD 
    <img src="images/jcad.png" alt="JupyterCAD logo" style="height:5rem; vertical-align:middle; margin:0 0.5rem;" />
    & 
    JupyterGIS 
    <img src="images/jgis.png" alt="JupyterGIS logo" style="height:5rem; vertical-align:middle; margin:0 0.5rem;" />
  </h2>

  <!-- JupyterGIS screenshot (bottom) -->
  <div style="position:absolute; top:15%; left:10%; width:60%; z-index:1;">
    <img src="images/jupytergis-ss.png" alt="JupyterGIS Screenshot" 
          style="width:100%; height:auto; border-radius:8px; box-shadow:0 4px 8px rgba(0,0,0,0.2);" />
  </div>

  <!-- JupyterCAD screenshot (top) -->
  <div style="position:absolute; top:30%; left:30%; width:60%; z-index:2;">
    <img src="images/jupytercad-ss.png" alt="JupyterCAD Screenshot" 
          style="width:100%; height:auto; border-radius:8px; box-shadow:0 4px 8px rgba(0,0,0,0.2);" />
  </div>

</section>




---

<section>
  <h3>About JupyterCAD</h3>
  <ul>
    <li >Browser-native 3D modeling for JupyterLab</li>
    <li >Built on <strong>OpenCascade</strong> (via WebAssembly) and <strong>ThreeJS</strong> for display</li>
    <li >Parametric, sketch-driven design</li>
    <li >Integrates with Python code cells</li>
  </ul>
</section>


<section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ACreate-Basic-Shapes.jcad"
      target="_blank"
      style="display: flex; align-items: center; gap: 0.5rem; text-decoration: none; color: inherit;"
    >
      <h2 style="text-transform: none; margin: 0;">JupyterCAD</h2>
      <img
        src="images/jcad.png"
        alt="JupyterCAD Logo"
        style="height: 1.5em; object-fit: contain; vertical-align: middle;"
      />
    </a>
  </div>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ACreate-Basic-Shapes.jcad"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>

<section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ACut-Example.jcad"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">Operations in Action</h3>
      <img
        src="images/jcad.png"
        alt="JupyterCAD Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem;">
    Cutting a box with spheres to create a nice shape
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ACut-Example.jcad"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>

<section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AMultiple-Views.jcad"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">Multiple Visualization Modes</h3>
      <img
        src="images/jcad.png"
        alt="JupyterCAD Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem; font-size: 1.9rem;">
    Switch between <strong>Exploded View</strong>, <strong>Clip Plane</strong>, and <strong>Wireframe</strong> to explore models in depth
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AMultiple-Views.jcad"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>

<section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ATransform-Controls.jcad"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">🎛️ Transform Controls with Snapping</h3>
      <img
        src="images/jcad.png"
        alt="JupyterCAD Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem;">
    Move, rotate, and snap with precision
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ATransform-Controls.jcad"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>

<section>
  <p><strong>🧮 Python API for programmatic geometry</strong></p>
  <p >Write Python code to generate & modify shapes</p>
  <video src="video/jcad/jcad-console.mp4" autoplay loop muted playsinline style="max-width: 90%; margin-top: 1rem;"></video>
</section>

<section>
  <p><strong>📓 Notebook integration</strong></p>
  <p >CAD alongside your code & documentation</p>
  <video src="video/jcad/jcad-notebook.mp4" autoplay loop muted playsinline style="max-width: 90%; margin-top: 1rem;"></video>
</section>

<section>
  <p><strong>🤝 Collaborative editing</strong></p>
  <p  style="font-size: 1.9rem">CRDT-based real-time co-editing via Y.js & PyCRDT</p>
  <video src="video/jcad/jcad-collaborative.mp4" autoplay loop muted playsinline style="max-width: 90%; margin-top: 1rem;"></video>
</section>

<section>
  <h3>💬 Suggestion Workflow</h3>
  <p style="font-size: 1.9rem">
    Like Github Pull Requests, Collaborators can review models — suggest, accept, or reject changes asynchronously.
  </p>
  <video src="video/jcad/jcad-suggestions.mp4" autoplay loop muted playsinline style="max-width: 90%; margin-top: 1rem;"></video>
</section>

<section>
  <h3>📁 File Format Support</h3>
  <ul>
    <li ><strong>FCStd</strong> — Read, edit, and export <em>FreeCAD</em> project files natively</li>
    <li ><strong>STL</strong> — Import mesh models for quick inspection or editing</li>
    <li ><strong>STEP</strong> — Bring in precise solid geometry from external CAD tools</li>
  </ul>
  <p  style="margin-top: 1rem;">
    Move between tools without friction — with support for common CAD formats.
  </p>
</section>

<section>
  <h3>JupyterCAD-MCP</h3>
  <video
    id="jupytercad-mcp-video"
    src="video/jcad/jupytercad-mcp.mp4"
    autoplay
    loop
    muted
    playsinline
    style="max-width: 90%; margin-top: 1rem;"
  ></video>

  <script>
    const video = document.getElementById('jupytercad-mcp-video');
    video.playbackRate = 2.0;
  </script>
</section>


---

<section>
  <h3>About JupyterGIS</h3>
  <ul>
    <li >A full-featured GIS toolkit inside JupyterLab</li>
    <li >Supports raster and vector layers</li>
    <li >Built with <strong>OpenLayers</strong> + <strong>GDAL</strong> (WebAssembly)</li>
  </ul>
</section>


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



<!-- Vertical stack for features -->
<section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AVector-Raster.jGIS"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">🗺️ Vector & Raster Data Support</h3>
      <img
        src="images/jgis.png"
        alt="JupyterGIS Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem; font-size: 1.9rem;">
    Load local and cloud-hosted vector & raster data directly
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AVector-Raster.jGIS"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>


<section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AVector-Symbology.jGIS"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">🖍️ Vector Symbology</h3>
      <img
        src="images/jgis.png"
        alt="JupyterGIS Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem;">
    Vector data with <strong>advanced</strong> rendering styles
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AVector-Symbology.jGIS"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>


  <section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ARaster-Symbology.jGIS"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">🖍️ Raster Symbology</h3>
      <img
        src="images/jgis.png"
        alt="JupyterGIS Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem;">
    Use <strong>singleband & multiband rendering</strong> to style raster datasets
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ARaster-Symbology.jGIS"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>


  <section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ADynamic-Management.jGIS"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">🔄 Dynamic Layer Management</h3>
      <img
        src="images/jgis.png"
        alt="JupyterGIS Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem;">
    Add, remove, and style layers using interactive UI
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ADynamic-Management.jGIS"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>


<section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AIdentify.jGIS"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">🔍 Identify Panel</h3>
      <img
        src="images/jgis.png"
        alt="JupyterGIS Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem;">
    Click features on map to inspect their attributes
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AIdentify.jGIS"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>



<section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ATime-Slider.jGIS"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">⏳ Time Slider</h3>
      <img
        src="images/jgis.png"
        alt="JupyterGIS Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem;">
    Visualize how data evolves over time
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3ATime-Slider.jGIS"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>


  <section>
  <h3>🧩 QGIS Compatibility</h3>
  <p >
    Import and export QGIS files, layers, and styles seamlessly.
  </p>
  <video src="video/jgis/jgis-qgis.mp4" autoplay loop muted playsinline style="max-width: 90%; margin-top: 1rem;"></video>
</section>

  <section>
  <h3>📝 Annotation & Collaboration</h3>
  <p>
    Add notes, draw shapes, and collaborate in real-time.
  </p>
  <video src="video/jgis/jgis-annotation.mp4" autoplay loop muted playsinline style="max-width: 90%; margin-top: 1rem;"></video>
</section>


  <section>
    <h3>📓 Notebook + Python Integration</h3>
    <p>Use Python code cells to add, style, and transform spatial layers</p>
    <video src="video/jgis/jgis-notebook.mp4" autoplay loop muted playsinline style="max-width: 90%; margin-top: 1rem;"></video>
  </section>

  <section>
  <div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin-bottom: 1rem;">
    <a
      href="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AProcessing.jGIS"
      target="_blank"
      style="display: flex; align-items: center; gap: 1rem; text-decoration: none; color: inherit;"
    >
      <h3 style="text-transform: none; margin: 0;">🧪 Client-Side Processing</h3>
      <img
        src="images/jgis.png"
        alt="JupyterGIS Logo"
        style="height: 50px; object-fit: contain;"
      />
    </a>
  </div>

  <p style="text-align: center; margin-bottom: 1rem;">
    Perform processing operations with GDAL-WASM
  </p>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html?path=RTC%3AProcessing.jGIS"
    style="
      border: none;
      width: 100vw;
      height: 75vh;
      transform: scale(0.9);
      transform-origin: top center;
    "
  ></iframe>
</section>

<section>
  <h3>📦 STAC Integration</h3>
  <p>
    Browse and visualize datasets directly from <strong>STAC catalogues</strong>
  </p>
  <video 
    src="video/jgis/jgis-stac.mp4" 
    autoplay 
    loop 
    muted 
    playsinline 
    style="max-width: 90%; margin-top: 1rem;"
  ></video>
</section>


<section>
  <h3>🌐 TiTiler Integration</h3>
  <p>
    Serve and explore vector & raster dynamically using <strong>Python + TiTiler</strong>
  </p>
  <video 
    src="video/jgis/jgis-titiler.mp4" 
    autoplay 
    loop 
    muted 
    playsinline 
    style="max-width: 90%; margin-top: 1rem;"
  ></video>
</section>


---

<section>
  <h2 style="text-transform: none;">Web Tech Under the Hood</h2>
  <ul>
    <li><strong>JupyterLab plugin</strong></li>
    <li><strong>PyCRDT + Y.js for collaboration</strong></li>
    <li><strong>WebAssembly (WASM) for processing</strong></li>
    <li><strong>Open Layers for visualization</strong></li>
  </ul>
</section>

<section style="position: relative; overflow: hidden;">
  <h2 style="text-transform: none;">JupyterLite support</h2>
  <ul>
    <li>Works in full JupyterLite setup</li>
    <li>Enables install-free use of JupyterGIS</li>
    <ul>
      <li>Client-side Python kernel</li>
      <li>Conda distribution <strong>emscripten-forge</strong></li>
      <li>WASM-based GDAL for processing</li>
    </ul>
    <li>All demos today were made on JupyterLite!</li>
    <li><strong>Check out the JupyterLite presentation at noon in this room!</strong></li>
  </ul>

  <img
    src="images/astronaut-victory.webp"
    alt="astronaut"
    style="
      position: absolute;
      bottom: 0;
      right: -140px;
      max-height: 80%;
      opacity: 0.3;
      pointer-events: none;
    "
  />
</section>


---

<section style="height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; padding:2rem;">
  <h2 style="text-align:center; margin-bottom:2.5rem;">Use Cases</h2>

  <div style="display:grid; grid-template-columns:1fr 1fr; gap:2rem; font-size:2.2rem; line-height:1.6;">
  
  <div>🌍 <strong>Environmental Science</strong><br><span style="color:#555;">Analyze climate or land-use patterns</span></div>
  <div>🌊 <strong>Geoscience</strong><br><span style="color:#555;">Map terrain, water or seismic data</span></div>
  <div>🛠️ <strong>Engineering</strong><br><span style="color:#555;">Parametric CAD models in notebooks</span></div>
  <div>📐 <strong>Education</strong><br><span style="color:#555;">Teach CAD/GIS with no installs</span></div>
  <div>⚡ <strong>R&D</strong><br><span style="color:#555;">Prototype & share browser-native apps</span></div>
  <div>🧑‍🤝‍🧑 <strong>Collaboration</strong><br><span style="color:#555;">Design reviews in the browser</span></div>

  </div>
</section>


---

<section style="height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; padding:2rem;">
  <h2 style="text-align:center; margin-bottom:2.5rem;">What's next for JupyterGIS?</h2>
  <h3 style="text-align:center; margin-bottom:2.5rem;">We have many ideas, help us make them real!</h3>

  <div style="display:grid; grid-template-columns:1fr 1fr; gap:2rem; font-size:2.2rem; line-height:1.6;">
  <div style="transform:rotate(-2deg) translateY(-5px); background:#fef9f5; padding:1.5rem 2rem; border-radius:1rem; font-size:1.7rem; box-shadow:0 4px 12px rgba(0,0,0,0.12);">
    <strong>MCP Server Extension</strong>
  </div>

  <div style="transform:rotate(1.5deg) translateY(8px); background:#f5fbff; padding:1.5rem 2rem; border-radius:1rem; font-size:1.7rem; box-shadow:0 4px 12px rgba(0,0,0,0.12);">
    <strong>Story Maps</strong>
  </div>

  <div style="transform:rotate(-1deg) translateY(4px); background:#f9f5ff; padding:1.5rem 2rem; border-radius:1rem; font-size:1.7rem; box-shadow:0 4px 12px rgba(0,0,0,0.12);">
    <strong>Suggestions Support</strong><br>(Split view comparison)
  </div>

  <div style="transform:rotate(2deg) translateY(-6px); background:#f5fff9; padding:1.5rem 2rem; border-radius:1rem; font-size:1.7rem; box-shadow:0 4px 12px rgba(0,0,0,0.12);">
    <strong>More Cloud Optimization</strong><br>(GeoParquet, GeoArrow)
  </div>

  <div style="transform:rotate(-1.5deg) translateY(5px); background:#fffdf5; padding:1.5rem 2rem; border-radius:1rem; font-size:1.7rem; box-shadow:0 4px 12px rgba(0,0,0,0.12);">
    <strong>Vector Layer Editing & Creation</strong>
  </div>

  <div style="transform:rotate(1deg) translateY(-4px); background:#f5f7ff; padding:1.5rem 2rem; border-radius:1rem; font-size:1.7rem; box-shadow:0 4px 12px rgba(0,0,0,0.12);">
    <strong>Advanced Table Viewer</strong>
  </div>
  </div>
</section>


---

<section>
  <h2 style="text-align:center;">🌍 Community & Contribution</h2>

  <p style="text-align:center;">
    🚀 <strong>Initial work on JupyterGIS</strong> was funded by <strong>ESA</strong><br>
    🌐 <strong>STAC browser & titiler extension</strong> were funded by <strong>CNES</strong>
  </p>

  <p style="text-align:center;">
    👩‍💻 Developed by <strong>QuantStack</strong>, <strong>Simula Research Lab</strong>, and <strong>DSE</strong>
  </p>
</section>

<section>
  <p style="text-align:center; font-size:1.1em; margin-top:1em;">
    👉 Join the <strong>GeoJupyter Community</strong>:
    <a href="https://geojupyter.org/" target="_blank">geojupyter.org</a>
  </p>

  <ul>
    <li>💻 Code contributions, bug fixes, plugin development</li>
    <li>📖 Documentation, tutorials, and example notebooks</li>
    <li>💡 Feedback, experience reports, feature requests</li>
  </ul>
</section>


---

<section style="display: flex; flex-direction: column; align-items: center; justify-content: flex-start; padding-top: 2rem;">
  <h2 style="text-transform: none;">Thank You</h2>
  <h3 style="margin-top: 2rem;">Questions?</h3>

  <div style="
    display: flex;
    justify-content: center;
    align-items: flex-start;
    gap: 100px;
    width: 100%;
  ">
    <div style="text-align: center;">
      <img src="images/jcad-qr.png" alt="JupyterCAD QR" style="width: 320px; height: auto;" />
    </div>
    <div style="text-align: center;">
      <img src="images/jgis-qr.png" alt="JupyterGIS QR" style="width: 350px; height: auto;" />
    </div>
  </div>
</section>
