# Part 1 - High-quality Offline Rendering of Objects

This deliverable consists of rendered images showcasing each object, created by individual group members, alongside shared background models, lighting, materials, and overall scene setup. All rendered images are designed to fit a cohesive theme and style. Incremental work, including sketches, early models, and pre-renders, will also be documented.

## 1 - Chair and Wardrobe  

### Modelling Process  

#### Chair Body  
The chair body was modeled from a basic cube, reshaped into an "L" by removing the top and front faces. Subdivision and solidify modifiers were applied to create a smooth, rounded finish. Loop cuts were added to define cushion edges, and the backrest was beveled for a softer look. In sculpt mode, dips and bulges were added for a cushion effect, enhanced with a cloth filter for softness.

#### Metal Rod, Legs, and Wheels  
The metal rod started as a cylinder, shaped with inset and extrusions to form sturdy ridges. Legs and wheels were modeled as cylindrical shapes with inset, extrusion, and loop cuts to create sections. The wheels and legs were combined into one object, duplicated with an array modifier, and rotated evenly using an empty object as a reference.

### Textures  

For the chair body, a leather texture was created using high-scale Noise Texture for grain and a Color Ramp for a warm brown color, with a Bump Node adding subtle surface imperfections. The metal rod texture used a procedural Noise Texture with FBM for fine detail, and a Color Ramp provided subtle color variation. The legs’ matte plastic texture was created with high- and low-scale Noise Textures for grain and diffuse patterns, while Color Ramps adjusted color variations, and a Bump Node added surface depth. Roughness was set to 1.0 for a realistic matte finish.

### Lighting & Camera  

### Render Output Settings 
- Render Engine: EEVEE
- Viewport Samples: 64 (Temporal Reprojection enabled, Jittered Shadows disabled)
- Render Samples: 4096
- Shadows: Rays - 3, Steps - 6, Volume Shadows Steps - 16, Resolution - 1.000
- Light Threshold: 0.010
- High-Quality Normals: Enabled


### Image link in Repo
https://github.com/Faiz-Iqbal/F20GA_Group7/blob/a8d3aca583ce0a6d8703e29a191b64057ed5ae7b/Render/Final_ChairAndWardrobe.jpg
