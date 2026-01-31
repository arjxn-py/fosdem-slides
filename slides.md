<!-- .slide -->
<div style="text-align: left; line-height: 1.2; position: relative;">

  <h2 style="font-size: 1.6em; margin: 0; font-weight: 600;">
    Interactive, Collaborative, <br/>
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
    Notebooks are <strong>reproducible</strong> computational documents.
  </p>

  <div style="display:flex; align-items:center; justify-content:center; gap:3rem; margin-top:2.5rem;">

<!-- Left: bullets -->
<ul style="flex:1; list-style-type:disc; font-size:1.4rem; line-height:1.8;">
    <li>Code, data, outputs, and narrative in one place</li>
    <li>Shareable, reproducible workflows</li>
    <li>Runs on desktop and in the browser</li>
</ul>

<!-- Right: visual -->
<div style="flex:1; text-align:center;">
    <img src="images/jupyterlab-screenshot.webp"
        alt="JupyterLab notebook"
        style="max-height:22rem; border-radius:8px; box-shadow:0 4px 12px rgba(0,0,0,0.2);" />
    <p style="font-size:1rem; margin-top:0.5rem;">
    Code • Output • Markdown
    </p>
</div>

  </div>

  <aside class="notes">
    In Jupyter, we already treat computation as a narrative.
    Everything is live, reproducible, and increasingly collaborative.
  </aside>
</section>


<section>
  <h2 style="text-align:center; font-size:2.5rem; margin-top:0.5rem;">
    Jupyter Collaboration
  </h2>

  <!-- Bullets on top -->
  <ul style="list-style-type:disc; font-size:1.6rem; line-height:2; margin:2rem auto; max-width:700px;">
    <li>Live multi-user editing</li>
    <li>Real-time updates</li>
    <li>No file conflicts</li>
  </ul>

  <!-- Image below -->
  <div style="width:90%; text-align:center; margin:0 auto;">
    <img src="images/jupyter-collab.png"
        alt="Jupyter real-time collaboration"
        style="width:100%; height:auto; border-radius:6px; box-shadow:0 4px 8px rgba(0,0,0,0.2);" />
    <p style="font-size:1.3rem; margin-top:0.5rem;">Live cursors • Shared outputs • Real-time sync</p>
  </div>
</section>



---

<section>
  <h2 style="text-align:center; margin-top:0.5rem;">
    What if GIS was a first-class citizen in JupyterLab?
  </h2>

  <p style="text-align:center; font-size:1.6rem; margin-top:1rem;">
    What if GIS documents were collaboratively editable like Jupyter notebooks?
  </p>

  <div style="display:flex; justify-content:center; align-items:center; gap:3rem; margin-top:3rem;">

  <img src="images/jupyter.svg" style="height:6rem;" />
  <span style="font-size:3rem;">+</span>
  <img src="images/gis.png" style="height:6rem;" />
  <span style="font-size:3rem;">+</span>
  <img src="images/collaboration-icon.png" style="height:6rem;" />

  </div>

  <aside class="notes">
    This is the core question behind JupyterGIS.
    We didn't want another plugin — we wanted a new model.
  </aside>
</section>


---

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


---

<section>
  <h1 style="
    text-align:center;
    font-size:6rem;
    letter-spacing:0.2rem;
    margin-top:20vh;
  ">
    DEMO
  </h1>

  <p style="
    text-align:center;
    font-size:1.8rem;
    margin-top:1rem;
    opacity:0.8;
  ">
    JupyterGIS in action
  </p>
</section>

<section>
  <div style="text-align:center; margin-bottom:1rem;">
    <h3 style="text-transform:none; margin:0;">
      Full JupyterGIS Environment
    </h3>
    <p style="font-size:1.4rem; opacity:0.8;">
      Live JupyterLab with JupyterGIS
    </p>
  </div>

  <iframe
    src="https://arjxn-py.github.io/myp/lab/index.html"
    style="
      border:none;
      width:100vw;
      height:80vh;
      transform:scale(0.9);
      transform-origin:top center;
    "
  ></iframe>
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

<section>
  <h2 style="text-align:center; font-size:2.8rem; margin-bottom:1rem;">
    📖 JupyterGIS StoryMaps (in progress)
  </h2>

  <p style="text-align:center; font-size:1.6rem; max-width:900px; margin:0 auto 2rem;">
    Compose interactive geospatial narratives by combining
    <strong>maps, text, and live data</strong>.
  </p>

  <div style="text-align:center;">
    <video
      src="video/jgis/jgis-storymap.mp4"
      autoplay
      loop
      muted
      playsinline
      style="max-width: 90%; border-radius:8px; box-shadow:0 4px 12px rgba(0,0,0,0.2);"
    ></video>
  </div>

  <aside class="notes">
    This is our vision for taking reproducible GIS beyond analysis:
    into communication, storytelling, and decision-making.
  </aside>
</section>

<section>
  <h2 style="text-align:center; font-size:2.8rem; margin-bottom:1rem;">
    🤖 LLM-powered GIS (in progress)
  </h2>

  <p style="text-align:center; font-size:1.6rem; max-width:900px; margin:0 auto 2rem;">
    Use natural language to explore, transform, and explain geospatial data
    inside JupyterGIS.
  </p>

  <div style="text-align:center;">
    <video
      src="video/jgis/jgis-llm.mp4"
      autoplay
      loop
      muted
      playsinline
      style="max-width: 90%; border-radius:8px; box-shadow:0 4px 12px rgba(0,0,0,0.2);"
    ></video>
  </div>

  <aside class="notes">
    This is about lowering the barrier to GIS.
    Instead of learning tools first, users start with questions.
  </aside>
</section>


---

<section style="position: relative; overflow: hidden;">
  <h2 style="text-transform: none;">JupyterLite support</h2>
  <ul>
    <li>All live demos today were made on JupyterLite!</li>
    <li>Works in full JupyterLite setup</li>
    <li>Enables install-free use of JupyterGIS</li>
    <ul>
      <li>Client-side Python kernel</li>
      <li>Conda distribution <strong>emscripten-forge</strong></li>
      <li>WASM-based GDAL for processing</li>
    </ul>
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

<section>
  <h2 style="text-transform: none; text-align:center; font-size:2.2rem;">
    Easiest way to try JupyterGIS instantly
  </h2>

  <div style="text-align:center; margin-top:0.5rem;">
    <img
      src="images/nblink.svg"
      alt="notebook.link"
      style="
        height:3rem;
        opacity:0.95;
      "
    />
  </div>

  <div style="text-align:center;">
    <video
      src="video/jgis/nblink.mp4"
      autoplay
      loop
      muted
      playsinline
      style="
        max-width: 80%;
        margin-top: 2rem;
        border-radius: 8px;
        box-shadow: 0 8px 24px rgba(0,0,0,0.25);
      "
    ></video>
  </div>
</section>



---

<section style="height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; padding:2rem;">
  <h2 style="text-align:center; margin-bottom:2.5rem;">
    Use Cases
  </h2>

  <div style="
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:2.2rem 3rem;
    font-size:2.1rem;
    line-height:1.5;
    max-width:1000px;
    margin: 0 auto;
  ">
  
  <div style="text-align:left;">
    🌍 <strong>Environmental Analysis</strong><br>
    <span style="color:#666;">Climate, land-use & biodiversity mapping</span>
  </div>

  <div style="text-align:left;">
    🛰️ <strong>Earth Observation</strong><br>
    <span style="color:#666;">STAC, satellite rasters, time series</span>
  </div>

  <div style="text-align:left;">
    🗺️ <strong>Urban & Mobility</strong><br>
    <span style="color:#666;">Infrastructure, zoning, accessibility</span>
  </div>

  <div style="text-align:left;">
    📐 <strong>Teaching & Workshops</strong><br>
    <span style="color:#666;">Zero-install, browser-based GIS</span>
  </div>

  <div style="text-align:left;">
    🧪 <strong>Reproducible Research</strong><br>
    <span style="color:#666;">Maps + code + narrative in one artifact</span>
  </div>

  <div style="text-align:left;">
    🤝 <strong>Collaborative Mapping</strong><br>
    <span style="color:#666;">Live multi-user spatial editing</span>
  </div>

  </div>
</section>


---

<section style="height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; padding:2rem;">
  <h2 style="text-align:center; margin-bottom:2.5rem;">What's next for JupyterGIS?</h2>
  <h3 style="text-align:center; margin-bottom:2.5rem;">We have many ideas, help us make them real!</h3>

  <div style="display:grid; grid-template-columns:1fr 1fr; gap:2rem; font-size:2.2rem; line-height:1.6;">

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
  <h2 style="text-align:center;">Community & Support</h2>

  <!-- Funders -->
  <div style="
    display:flex;
    justify-content:center;
    gap:4rem;
    margin:2.5rem auto 1.5rem auto;
    align-items:center;
    flex-wrap:wrap;
  ">
    <img src="images/logo-qs.svg" style="height:50px; object-fit:contain;" />
    <img src="images/esa.png" style="height:100px; object-fit:contain;" />
    <img src="images/simula.webp" style="height:50px; object-fit:contain;" />
    
  </div>

  <p style="text-align:center; font-size:1.3rem; margin-top:1.5rem;">
    Initial development funded by <strong>ESA</strong> under permanent open call for EO innovation.<br>
    STAC & xarray extension funded by <strong>CNES</strong>
  </p>

  <p style="text-align:center; font-size:1.2rem; margin-top:1rem;">
    Built by <strong>QuantStack</strong> & <strong>Simula Research Lab</strong><br>
    With major contributions from <strong>UC Berkeley DSE</strong>
  </p>

  <p style="text-align:center; font-size:1.1rem; margin-top:1.5rem; opacity:0.8;">
    And over 30 open-source contributors.
  </p>

  <!-- Builders / Contributors -->
  <div style="
    display:flex;
    justify-content:center;
    gap:3rem;
    margin-bottom:2rem;
    align-items:center;
    flex-wrap:wrap;
  ">
    <img src="images/cnes.png" style="height:100px; object-fit:contain;" />
    <img src="images/dse.png" style="height:100px; object-fit:contain;" />
    <img src="images/contributors.png" style="height:150px; object-fit:contain;" />
  </div>
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
