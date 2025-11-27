# OpenGL Scene Engine

This project implements an interactive **3D scene engine** capable of rendering environments from a custom `.ray` scene-description format.  
Using textures, materials, lighting definitions, and parametric geometry, the engine produces realistic indoor scenes that can be explored interactively with a movable camera.

This repository showcases two example scenes I built using the engine:  
a furnished **room environment** and a stylized **basketball shot**.

---

## Features

### Scene description language
Scenes are defined by human-readable `.ray` files specifying:
- Geometry (sphere, torus, triangle meshes, box, etc.)
- Material properties (ambient / diffuse / specular / shininess)
- Lighting configurations (point / directional / spot)
- Texture bindings
- Camera parameters

### Texture-mapped 3D geometry
Materials support:
- JPEG textures
- Per-vertex UV mapping
- Multi-material scenes
- Glossiness and emissive highlights

### Physically inspired lighting
Scenes can include multiple lights at once:
- Point lights
- Directional lights
- Spotlight effects

### Interactive exploration (in the full engine)
The engine allows:
- Camera translation (forward/back, strafe, vertical)
- "Crystal-ball" rotation style orbit around objects
- Smooth navigation with sensitivity scaling based on world distance

---

## Render Gallery

### Authored Scenes
| Globe (UV texture mapping) | Basketball (authored scene) |
|----------------------------|-----------------------------|
| <img src="globeoutput.png" width="420"/> | <img src="artcontestoutput.png" width="420"/> |

### Additional Models Rendered with the Engine
| Dragon (triangle mesh) | Nefertiti (triangle mesh) |
|------------------------|---------------------------|
| <img src="dragonoutput.png" width="420"/> | <img src="nefertitioutput.png" width="420"/> |

Note: Mesh scene files (dragon, nefertiti) were provided as part of a graphics course and are not included here. Screenshots shown here were generated using my implementation of the renderer.

---

## Scene files

This repository contains two authored `.ray` scenes:

| File | Description |
|------|-------------|
| `globe.ray` | Textured spherical Earth model illuminated by a directional “sun” light source over a reflective material floor |
| `basketball.ray` | Basketball scene using a torus hoop and textured sphere |

Both scenes demonstrate:
- Texture mapping
- Lighting & shadows
- Parametric geometry
- Material variation

---

## Repository structure

/scenes → Authored .ray scene files
/textures → Textures used by the scenes
/screenshots → Render output images
README.md

yaml

⚠️ Note: This repository intentionally does **not** include course-provided framework code.

---

## 🔐 Source Code Access

The full **C++ OpenGL implementation** (my `.todo.cpp` rendering code) is stored in a **private repository** to respect academic integrity policies.

If you are an interviewer or someone interested and would like to review the implementation, please reach out.

## Technical Skills Highlighted

- C++  
- OpenGL (fixed-function graphics pipeline)  
- 3D rendering & camera math  
- Texture mapping & lighting models  
- Scene graph representation  
- Asset handling & material systems

---

## Future Improvements

- Modern OpenGL + GLSL shaders
- Shadow maps
- Normal mapping / PBR materials
- Real-time UI for light toggling and scene editing

---

## Contact

If you’d like to talk about this project or view the full implementation:

**Lilah Dicker**  
📧 *ldicker6@jh.edu*  

