# 3d Models imbeded

## HTML Structure

We’ll create a container div to host the WebGL canvas:

```bash
<div id="threejs-container" style="width:600px; height:400px;"></div>
```
- You can create multiple containers on the page; each can have its own 3D viewer.

- The width and height control canvas size.

## Reusable JS Function

a function init3DViewer(containerId, modelUrl) that:

- Creates renderer, scene, camera

- Loads the model

- Centers & scales it

- Adds OrbitControls

- Supports transparent background

## Usage Example

``` bash
<div id="viewer1" style="width:600px; height:400px;"></div>
<div id="viewer2" style="width:400px; height:300px;"></div>

<script type="module">
import { init3DViewer } from "./threeViewer.js";

// Viewer 1
init3DViewer("viewer1", "/cool_cup.glb");

// Viewer 2 (different model)
init3DViewer("viewer2", "/another_model.glb");
</script>
```

[page](https://hamidspirit.github.io/3d/)
