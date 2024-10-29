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
All objects are positioned slightly above the ground to emphasize shadow effects from the 3-point lighting setup.

### Render Output Settings 
- Render Engine: EEVEE
- Viewport Samples: 16 (Temporal Reprojection enabled, Jittered Shadows disabled)
- Render Samples: 1024
- Shadows: Enabled
- High-Quality Normals: Enabled
- Memory:
  - Shadow Pool: 1 GB
  - Light Probes Volume: 64 MB
- Viewport Pixel Size: 4x

### Image link in Repo
https://github.com/Faiz-Iqbal/F20GA_Group7/blob/a8d3aca583ce0a6d8703e29a191b64057ed5ae7b/Render/Final_ChairAndWardrobe.jpg

## 2 - Bed and Plant  

### Modelling Process  

#### Bed  
The bed frame was modeled from a scaled cube, with an extrusion on top for the headboard. A bevel modifier was applied to smooth the edges. The mattress was created by scaling a cube, subdividing it, and adding cloth physics for a cushion effect, along with a collision modifier. Pillows were modeled similarly to the mattress, excluding the collision modifier. For the bedsheet, a plane was added, subdivided, and cloth physics were applied. The plane was rotated on the Y-axis before running the simulation to create natural wrinkles. A solidify modifier was then added to provide thickness.

#### Plant  
The plant's leaves were modeled from a scaled cube, with edge loops and a subdivision modifier for added detail. Leaves were duplicated and layered to create a natural arrangement. The pot was created from a circle mesh, shaped with extrusions, and the dirt was made from another circle mesh with subdivisions and a displace modifier to add roughness.

### Textures  

For the bed, the frame was textured with procedural nodes to create a wood effect, using noise and color for grain, along with bump and displacement for added detail. The mattress texture was kept simple, as it is mostly hidden. The bedsheet texture utilized a woven fabric pattern, created with two Wave Textures (aligned on the X and Y axes) connected through a Texture Coordinate node, combined with a Mix Node and enhanced with a Bump Node for surface detail. The pillows used image textures for color, roughness, and displacement, connected to a BSDF Shader. 

For the plant, a mix of diffuse and glossy shaders was applied to the leaves for a subtle shine. The pot used a noise texture with a bump node for texture. The dirt was textured with a noise texture and bump node for a rough, realistic look.

### Lighting & Camera  
All objects are positioned slightly above the ground to emphasize shadow effects from the 3-point lighting setup.

### Render Output Settings  
- Render Engine: EEVEE
- Viewport Samples: 16 (Temporal Reprojection enabled, Jittered Shadows disabled)
- Render Samples: 1024
- Shadows: Enabled
- High-Quality Normals: Enabled
- Memory:
  - Shadow Pool: 1 GB
  - Light Probes Volume: 64 MB
- Viewport Pixel Size: 4x

### Image link in Repo
https://github.com/Faiz-Iqbal/F20GA_Group7/blob/fc8266970a851c54b1d7d855c290e14c0ccb25d7/Render/Final_BedAndPlant.jpg

## 3 - Table and Lamp  

### Modelling Process  

#### Table  
The table was constructed starting with a cube for the tabletop, scaled to the correct dimensions. The legs were adjusted separately to achieve the desired thickness and height. Loop cuts were added to create drawer details, with faces extruded and handles slightly inset for realism. An array modifier was applied to replicate drawer units evenly, followed by a bevel modifier for smooth edges. On the right side, shelves were created and supported by cylindrical pillars, with segments added for smooth shaping. The table was then finished with a metallic material, polished for a smooth look.

#### Lamp  
The lamp stand was modeled from a cylinder, using Loop Tools for smooth transitions. The lampshade was hollowed out with the Bool Tool and additional edge loops were added for refined edges. Key parts like the stand and lampshade had a subdivision surface modifier applied for smoother geometry without losing sharp details. The bulb was created from the hollowed-out interior of the lampshade, shaped to resemble a bulb, and given an emissive material to simulate a glow. Additional books were modeled from cubes, with individual pages and cover details added for realism.

### Textures  

- **Wood Textures**: Created using a Noise Texture with Mapping for control, refined with a Color Ramp. This setup was connected to a Principled BSDF for the base color, with a Bump Node and Displacement Node adding surface depth and detail.
- **Drawers**: Utilized a Color Ramp for base color control, feeding into a Principled BSDF shader with adjusted roughness for a natural finish.
- **Metal Rods**: Used a Noise Texture connected to a Bump Node to add surface detail. The setup fed into a Principled BSDF with high metallic and low roughness values, creating a realistic metal bar appearance.
- **Rest of Objects**: Textured with a Principled BSDF shader, adjusted with a diffuse base color and minor tweaks for a simple yet effective material appearance.

### Lighting & Camera  
All objects are positioned slightly above the ground to enhance shadow effects using a 3-point lighting setup.

### Render Output Settings  
- Render Engine: EEVEE
- Viewport Samples: 16 (Temporal Reprojection enabled, Jittered Shadows disabled)
- Render Samples: 1024
- Shadows: Enabled
- High-Quality Normals: Enabled
- Memory:
  - Shadow Pool: 1 GB
  - Light Probes Volume: 64 MB
- Viewport Pixel Size: 4x

### Image link in Repo
https://github.com/Faiz-Iqbal/F20GA_Group7/blob/7e3057dae7e6209429d107486e24a6e2d74ac71c/Render/Final_Render_Table%26Lamp.jpg

## Final Isometric Room Render  

The final room render includes additional details to enhance realism. A window was created using an Emission Shader applied to a cube, giving the appearance of natural light entering the room. A dustbin was modeled from a cylinder mesh, scaled and extruded for the shape, with paper balls crafted by manipulating vertices of a sphere in Edit Mode for an irregular, crumpled look. Only the carpet and picture frame were imported assets, keeping the rest of the objects custom-made.

Link to Image in Repo: https://github.com/Faiz-Iqbal/F20GA_Group7/blob/7e3057dae7e6209429d107486e24a6e2d74ac71c/Render/Final_Isometric_Room.jpg

### Final Render Output Settings  
- Render Engine: EEVEE
- Viewport Samples: 64 (Temporal Reprojection enabled, Jittered Shadows disabled)
- Render Samples: 4096
- Shadows: Rays - 3, Steps - 6, Volume Shadows Steps - 16, Resolution - 1.000
- Light Threshold: 0.010
- High-Quality Normals: Enabled

## Overall Camera & Lighting  

The camera was positioned at an angle to capture a clear, comprehensive view of the entire room setup. A traditional 3-point lighting setup was employed with a 2:1:0.5 ratio, using Area Lights for each source. The Key Light provided primary illumination and defined shadows, the Fill Light softened shadows and balanced the lighting, and the Back Light added separation and depth to the scene. Additionally, spotlights were strategically placed in various locations to emphasize specific details. The scene was rendered using the Eevee render engine, chosen for its real-time performance, making it ideal for quick previews and the final render.
