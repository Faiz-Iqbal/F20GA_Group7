# Table of Contents
- [1 - Chair and Wardrobe](#1---chair-and-wardrobe)
- [2 - Bed and Plant](#2---bed-and-plant)
- [3 - Table and Lamp](#3---table-and-lamp)
- [4 - Final Isometric Room Render](#4---final-isometric-room-render)
- [5 - Overall Camera & Lighting](#5---overall-camera--lighting)

# Part 1 - High-quality Offline Rendering of Objects

This deliverable consists of rendered images showcasing each object, created by individual group members, alongside shared background models, lighting, materials, and overall scene setup. All rendered images are designed to fit a cohesive theme and style. Incremental work, including sketches, early models, and pre-renders, is also documented.

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

### Image
![Chair & Blender](https://github.com/Faiz-Iqbal/F20GA_Group7/blob/819eee9c1b8017acdcc08d1b47760f6022b860cd/Render/Final_ChairAndWardrobe.jpg)

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
![Bed & Plant](https://github.com/Faiz-Iqbal/F20GA_Group7/blob/819eee9c1b8017acdcc08d1b47760f6022b860cd/Render/Final_BedAndPlant.jpg)

## 3 - Table and Lamp  

### Modelling Process  

#### Table  
The table was constructed starting with a cube for the tabletop, scaled to the correct dimensions. The legs were adjusted separately to achieve the desired thickness and height. Loop cuts were added to create drawer details, with faces extruded and handles slightly inset for realism. An array modifier was applied to replicate drawer units evenly, followed by a bevel modifier for smooth edges. On the right side, shelves were created and supported by cylindrical pillars, with segments added for smooth shaping. The table was then finished with a metallic material, polished for a smooth look.

#### Lamp  
The lamp stand was modeled from a cylinder, using Loop Tools for smooth transitions. The lampshade was hollowed out with the Bool Tool and additional edge loops were added for refined edges. Key parts like the stand and lampshade had a subdivision surface modifier applied for smoother geometry without losing sharp details. The bulb was created from the hollowed-out interior of the lampshade, shaped to resemble a bulb, and given an emissive material to simulate a glow. Additional books were modeled from cubes, with individual pages and cover details added for realism.

### Textures  
Wood textures were created using a Noise Texture with Mapping for control, refined with a Color Ramp, and connected to a Principled BSDF for the base color, while a Bump Node and Displacement Node added surface depth and detail. The drawers used a Color Ramp for base color control, feeding into a Principled BSDF shader with adjusted roughness for a natural finish. For the metal rods, a Noise Texture connected to a Bump Node added surface detail, with a Principled BSDF shader set to high metallic and low roughness values for a realistic metal appearance. The rest of the objects were textured with a Principled BSDF shader, adjusted with a diffuse base color and minor tweaks to create a simple yet effective material look.

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

### Image
![Table and Lamp](https://github.com/Faiz-Iqbal/F20GA_Group7/blob/819eee9c1b8017acdcc08d1b47760f6022b860cd/Render/Final_Render_Table%26Lamp.jpg)

## 4 - Final Isometric Room Render  

The final room render includes additional details to enhance realism. A window was created using an Emission Shader applied to a cube, giving the appearance of natural light entering the room. A dustbin was modeled from a cylinder mesh, scaled and extruded for the shape, with paper balls crafted by manipulating vertices of a sphere in Edit Mode for an irregular, crumpled look. Only the carpet and picture frame were imported assets, keeping the rest of the objects custom-made.

### Final Image
![Isometric Room Render](https://github.com/Faiz-Iqbal/F20GA_Group7/blob/bf8a95a346dfca112b5d76e7b8894dbca6fa1b4a/Render/Final_Isometric_Room.jpg)

### Final Render Output Settings  
- Render Engine: EEVEE
- Viewport Samples: 64 (Temporal Reprojection enabled, Jittered Shadows disabled)
- Render Samples: 4096
- Shadows: Rays - 3, Steps - 6, Volume Shadows Steps - 16, Resolution - 1.000
- Light Threshold: 0.010
- High-Quality Normals: Enabled

## 5 - Overall Camera & Lighting  

The camera setup was carefully positioned at an elevated angle to provide a comprehensive view of the entire room, ensuring all key elements were visible while maintaining a balanced composition. The chosen angle highlights the spatial relationships between objects and creates a visually engaging perspective, capturing the depth and layout of the scene. This positioning also allowed an effective demonstration of the lighting setup, showing shadow falloff and object highlights.

A traditional 3-point lighting setup was employed to achieve balanced and realistic lighting, using a 2:1:0.5 intensity ratio between the Key, Fill, and Back Lights. 

**Key Light**: Positioned at a high angle in front of the main focal area, the Key Light served as the primary source of illumination, set at twice the intensity of the Fill Light to establish the dominant lighting direction. The Key Light was angled to cast clear directional shadows, defining the texture and contours of key objects such as the table, chair, and bed. This light was also adjusted to enhance the textures on surfaces, like wood grain on the table and the fabric on the chair, providing sharp, well-defined shadows that added realism and depth to the scene.

**Fill Light**: The Fill Light was placed opposite the Key Light, at half the Key Light’s intensity, to soften shadows and reduce contrast in the darker areas of the room. This light helped distribute the illumination more evenly, preventing harsh contrasts and preserving details in the shadowed areas. By providing a balanced light across the scene, the Fill Light kept the atmosphere natural while ensuring that secondary elements, such as shelves and smaller items, were subtly highlighted without taking attention away from the main focal points.

**Back Light**: Positioned behind and slightly above the main objects, the Back Light provided a soft glow that separated the objects from the background, enhancing the scene's depth. Set at a low intensity (0.5 times the strength of the Key Light), it created delicate highlights along the edges of objects, accentuating contours and enhancing the sense of space. This subtle rim lighting was particularly effective for objects with defined shapes, like the chair back, lamp, and shelves, providing a sense of dimension and realism without overpowering the scene.

In addition to the 3-point lighting setup, spotlights were strategically placed to enhance specific areas. For example, a spotlight focused on the table area emphasized the metallic and wood textures, while another directed at the plant brought out details in the leaves and pot. These spotlights provided localized highlights, adding visual interest and guiding the viewer’s attention around the room.

The entire lighting setup was optimized for the Eevee render engine, selected for its real-time rendering capabilities and speed. This engine allowed for rapid adjustments and previews, enabling fine-tuning of both lighting and composition. High sample rates and optimized shadow settings were used to enhance the visual quality of the final render, ensuring crisp shadows and minimal noise. Eevee’s blend of real-time feedback and quality results made it ideal for creating the intended atmosphere and achieving a polished, professional final render.
