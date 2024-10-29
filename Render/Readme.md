# Part 1 - High-quality Offline Rendering of Objects

This deliverable consists of rendered images showcasing each object, created by individual group members, alongside shared background models, lighting, materials, and overall scene setup. All rendered images are designed to fit a cohesive theme and style. Incremental work, including sketches, early models, and pre-renders, will also be documented.

## 1 - Chair and Wardrobe  

### Modelling Process  

#### Chair Body  
The chair's body began as a simple cube with the top and front faces deleted to form an L-shape base for the chair. Subdividing the mesh allowed for smooth curves, which were further enhanced by applying a subdivision surface modifier for a rounded finish. A solidify modifier was added for thickness, and loop cuts were used to create cushion borders, defining the edges. 

The backrest segment includes a beveled edge for added softness, complemented by auto smooth shading. Sculpt mode adjustments, such as shrinking the face set into smaller segments, introduced dips and bulges, which were further refined with a cloth filter to achieve a cushion-like texture. This completed the chair body.

#### Metal Rod, Legs, and Wheels  
The metal rod began as a basic cylinder. Using the inset tool, an inner face was created, followed by multiple extrusions along the rod, with scale adjustments at each step to form ridges and create a sturdy base.

The legs were modeled as cylindrical shapes with wheels attached, formed through inset, extrusion, and loop cuts. To simplify, the wheel and leg were joined as a single object. The array modifier was then applied to create five evenly spaced legs. An empty object was used as a rotation reference point to ensure accurate spacing, with the array modifier’s eyedropper tool set to this empty axis. This allowed the legs to be evenly rotated and spaced, completing the chair’s basic structure for texturing.

### Textures  

#### Leather for Chair Body  
The leather texture for the chair body uses Texture Coordinate and Mapping nodes to ensure consistent mapping across the material. A high-scale Noise Texture provided a fine grain effect, creating leather-like roughness. A Color Ramp adjusted the color to a warm brown tone and was connected to the Base Color.

To introduce depth and realism, a Bump Node driven by a second Color Ramp added small surface imperfections. The setup was linked to the Principled BSDF Shader and Material Output, resulting in a leather texture with realistic color and tactile detail.

#### Metal Rod  
The metal rod texture was created using a procedural approach. Starting with Texture Coordinate and Mapping nodes for precise control, a Noise Texture set to Fractal Brownian Motion (FBM) added fine surface detail. A Color Ramp adjusted the color variation, creating a subtle metallic look. 

For added surface depth, a Bump Node driven by another Color Ramp was connected to simulate minor imperfections, achieving a polished metal effect. The setup was finalized by adjusting the Principled BSDF Shader’s Metallic and Roughness settings and linking to the Material Output.

#### Matte Plastic for Legs  
The legs’ matte plastic texture was generated procedurally with Texture Coordinate and Mapping nodes, eliminating the need for UV mapping. Two Noise Texture nodes were connected to prevent a completely smooth finish.

The first Noise Texture was set to a high scale (100) for a fine grain, while the second was set to a lower scale (30) for larger, diffuse patterns, enhancing the matte effect with soft depth. Two Color Ramps controlled the color from dark gray to near-black and linked to a Bump Node for subtle depth. The Principled BSDF Shader had a roughness set to 1.0 for a non-glossy finish, connected to the Material Output, providing a realistic matte plastic texture with slight imperfections.

### Lighting & Camera  


### Render Output Settings 

### Image link in Repo
https://github.com/Faiz-Iqbal/F20GA_Group7/blob/a8d3aca583ce0a6d8703e29a191b64057ed5ae7b/Render/Final_ChairAndWardrobe.jpg
