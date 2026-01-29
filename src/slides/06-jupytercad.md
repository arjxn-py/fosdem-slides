<!-- <section>
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
</section> -->
