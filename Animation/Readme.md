# ONE DRIVE LINK: https://heriotwatt-my.sharepoint.com/:f:/r/personal/mm2046_hw_ac_uk/Documents/BSc%20Computer%20Science%20(Artificial%20Intelligence)/Academic%20Year%204/F20GA%20-%203D%20Graphics%20and%20Animation/Shared_Files/F20GA_Group7_CourseworkUploads?csf=1&web=1&e=UGtrtt


# Part 2 - A video sequence animation of your scene.
Export your models from the modelling tool into Unreal Engine. Replace and fix any pipeline problems (e.g., light sources, textures, positions) and animate an interesting video sequence using the Engine, Blueprints and Sequencer. Save this animation as a video. You need to use animation concepts, same models, and keep the output video short to less than 1 minute long.

# Isometric Room Animation Project

This README provides a comprehensive overview of the **Isometric Room Animation Project**, highlighting the key stages of design, modeling, animation, and final rendering. We used Blender and Unreal Engine to bring a realistic isometric room to life.

---

## 1 - Project Overview

We embarked on designing a realistic and visually appealing isometric room using Blender. After experimenting with both FBX and glTF formats for model export, we selected **FBX** for its compatibility with Unreal Engine. Prior to export, all models were UV unwrapped as necessary.

Upon importing the FBX files into Unreal Engine, using the "Film/Video & Live Events" setting, we encountered and resolved several issues:

- **Wardrobe Rendering Issue**: The top part appeared hollow. We adjusted the material settings to "Two-sided" to ensure solidity.
- **Wardrobe Handles Quality**: Post-import, the handles did not meet our quality expectations. We remodeled them directly in Unreal Engine and applied the desired materials.
- **Bedsheet Texture Challenges**: The ruffled texture did not translate well. We reverted to an earlier Blender model without ruffles(using our git repo), re-exported it, and updated the model in Unreal with new textures to better suit our goals.

Additionally, we incorporated walls from the "Architecture" folder within Unreal's starter content. Missing textures were manually assigned from Unreal’s extensive library, and some of the material nodes were fine-tuned to achieve the desired effects. With all textures applied and materials adjusted, our isometric room was prepared for the animation stage.

---

## 2 - Animation Process

In Unreal Engine's Sequencer, we added a new level sequence to animate each object individually, utilizing features like transform, camera components, and light components. Key animation concepts applied include:

- **Window Blinds**: Each blind appears sequentially from the left and right, creating a smooth, cascading effect.
- **Bed**: The bed frame and mattress scale up together, followed by the bedsheet, then pillows rotate and descend from above.
- **Wardrobe**: The body appears from the left and handles from the right, employing linear motion without pre-defined keyframes.
- **Table Setup**: The table appears from the back, with the PC scaling into position, followed by the lamp. The lamp's light turns on and off at intervals, demonstrating timing variations.
- **Books**: Books fly into the scene, rotating at different speeds, adding visual interest and variety.
- **Chair**: The chair scales from zero to its correct size and then rotates on its axis from one place to another at varying speeds, ensuring smooth transitions in motion.
- **Dustbin**: The dustbin scales up from zero and positions itself, while paper balls simultaneously scale to size and fall into it, emphasizing their impact.
- **Plant Pot**: The plant pot scales from zero to full size, followed by the sequential appearance of the leaves, ensuring each leaf is distinctly visible.

---

## 3 - Lighting Setup

Our animation utilizes multiple light sources to clearly showcase all objects, enhancing textures, shadows, and reflections:

- **Sun (Directional Light)**: Simulates natural daylight with an intensity of 2, casting consistent shadows across the room.
- **3-Point Light System**:
  - **Key Light**: Intensity of 3000 lumens with a wide cone angle, illuminating main areas like the desk and bed.
  - **Fill Light**: Also set to 3000 lumens, softening shadows to prevent complete darkness in shaded areas.
  - **Back Light**: Positioned behind objects, adding a rim of light to separate items like the wardrobe and bed from the background.
- **Atmospheric Fog**: Utilized to improve the contrast of all textures.

---

## 4 - Camera Configuration

We opted for the **Cinema Camera Actor**, allowing us to set multiple tracking points for each object, facilitating focused zooms and movements. The camera remains stationary during object animations, moving closer from the succulent plant onwards to highlight finer details before returning to its original position. Settings include:

- **Aspect Ratio**: 16:9 Digital Film for a cinematic look.
- **Focal Length**: 35mm for a natural field of view.
- **Aperture**: Set to 2.8, creating a shallow depth of field to draw attention to specific objects while subtly blurring the background.

---

## 5 - Final Rendering Output

For the final sequence render, we installed **FFmpeg**, an open-source encoder. Output settings:

- **Format**: MP4 with libx264 for video and AAC for audio.
- **Resolution**: Full HD at 1920x1080.
- **Frame Rate**: 24 fps, balancing quality and file size for GitHub.

---

