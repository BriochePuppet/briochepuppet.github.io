# Brioche Puppet  

I am currently working on the free and open-source **VTuber** software **Brioche Puppet**.  

As a rendering engineer, the **rendering** is implemented by myself. But the third-party libraries [JoltPhysics](https://github.com/HanetakaChou/JoltPhysics) and [MeidaPipe](https://github.com/HanetakaChou/mediapipe) are used for **ragdoll physics** and **motion capture**.  

## 1\. Asset Import  
  
[Brioche Asset Import](https://github.com/HanetakaChou/Brioche-Asset-Import)  

### 1-1\. Mesh and Animation  

- [ ] [MMD (PMX, VMD)](https://github.com/UuuNyaa/blender_mmd_tools/tree/main)  
- [ ] [glTF (glTF, glB, VRM, VRMA)](https://github.com/saturday06/VRM-Addon-for-Blender/blob/main/src/io_scene_vrm/common/human_bone_mapper/mmd_mapping.py)  

### 1-2\. Image  

#### 1-2-1\. [Albedo Image](https://www.pbr-book.org/4ed/Radiometry,_Spectra,_and_Color/Color#FromRGBtoSpectra)  

- [x] [WebP](https://chromium.googlesource.com/webm/libwebp)  
- [x] [PNG](https://github.com/pnggroup/libpng)  
- [x] [JPEG](https://github.com/libjpeg-turbo/libjpeg-turbo)  

#### 1-2-2\. [Illuminant Image](https://www.pbr-book.org/4ed/Radiometry,_Spectra,_and_Color/Color#x6-RGBIlluminants)  

- [ ] [OpenEXR](https://github.com/AcademySoftwareFoundation/openexr)  

### 1-3\. Environment Map (Environment Lighting Image)  

- [ ] [Equirectangular (Latitude-Longitude) Map](https://www.pbr-book.org/3ed-2018/Light_Sources/Infinite_Area_Lights)  
- [ ] [Octahedral Map](https://www.pbr-book.org/4ed/Light_Sources/Infinite_Area_Lights#ImageInfiniteLights)  
- [ ] [~~Cube Map~~](https://dev.epicgames.com/documentation/en-us/unreal-engine/creating-cubemaps?application_version=4.27)  

## 2\. Motion    
    
[Brioche Motion](https://github.com/HanetakaChou/Brioche-Motion)  

### 2-1\. Motion Capture  
- [x] Video Capture  
- [x] Motion Detector  

### 2-2\. Animation  
- [ ] ~~Animation Retargeting~~      
- [ ] IK (Inverse Kinematics)  
    - [ ] Reaching IK (Target Position)  
        - [ ] Two Joints IK  
        - [ ] Three Joints IK  
        - [ ] ~~CCD (Cyclic Coordinate Descent) IK~~  
        - [ ] FABRIK (Forward And Backward Reaching Inverse Kinematics)  
        - [ ] Foot IK  
    - [ ] Aim IK (Target Direction)  
        - [ ] Look At IK  
- [ ] Ragdoll Physics  

## 3\. Rendering  

[Brioche ANARI](https://github.com/HanetakaChou/Brioche-ANARI)  
  
### 3-1\. Rasterization  

- [x] [PBR (Microfacet Model: Trowbridge Reitz)](https://pharr.org/matt/blog/2022/05/06/trowbridge-reitz)  
- [ ] [~~Toon Shading~~](https://github.com/unity3d-jp/UnityChanToonShaderVer2_Project)  
- [ ] [~~SSS (Skin: Subsurface Scattering)~~](https://zero-radiance.github.io/post/sampling-diffusion/)  
- [ ] [~~LTC (Area Lighting: Linearly Transformed Cosine)~~](https://github.com/selfshadow/ltc_code)  
- [x] [IBL (Environment Lighting: Spherical Harmonics + Split Sum Approximation)](https://github.com/HanetakaChou/Environment-Lighting)  
- [ ] [~~VXGI (Global Illumination: Clipmap Cone Tracing)~~](https://dl.acm.org/doi/abs/10.1145/2775280.2792546)  

### 3-2\. Ray Tracing  
- [ ] [ReSITR (Reservoir-Based Spatiotemporal Importance Resampling)](https://intro-to-restir.cwyman.org/)  
- [ ] [~~SVGF (Denoiser: Spatiotemporal Variance Guided Filtering)~~](https://github.com/NVIDIA-RTX/NRD)  
- [ ] [~~SSS (Skin: Subsurface Scattering)~~](https://github.com/NVIDIA-RTX/RTXCR/blob/main/docs/RtxcrSssGuide.md)  
- [ ] [~~SHaRC (Spatially Hashed Radiance Cache)~~](https://github.com/NVIDIA-RTX/SHARC)  

### 3-3\. Nerual Rendering  
- [ ] [~~NS (Nerual Shading)~~](https://github.com/NVIDIA-RTX/RTXNS/blob/main/docs/ShaderTraining.md)  
- [ ] [~~NeRF (Neural Radiance Fields)~~ ](https://www.matthewtancik.com/nerf)  
- [ ] [~~NRC (Neural Radiance Cache)~~](https://github.com/NVIDIA-RTX/NRC)  
