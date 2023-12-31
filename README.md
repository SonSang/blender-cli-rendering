# blender-cli-rendering

![GitHub](https://img.shields.io/github/license/yuki-koyama/blender-cli-rendering)
![Blender](https://img.shields.io/badge/Blender-2.93-brightgreen)

A set of Blender Python scripts for generating scenes and rendering images directly from command-line interface.

## Principles

- Able to run without display (thus, the renderer should be Cycles instead of EEVEE)
- Support the latest LTS release (currently 2.93)

## Possible Usages

- Material to learn how to use Blender Python APIs.
- Visualization of 3D data with fancy rendering quality.
- Generation of synthetic training datasets for machine learning-based computer vision.

## Blender Install

Download Blender 2.93 LTS by
```bash
wget https://mirror.clarkson.edu/blender/release/Blender2.93/blender-2.93.18-linux-x64.tar.xz
tar -xvf blender-2.93.18-linux-x64.tar.xz
```

Add the following line to `~/.bashrc`:
```bash
export PATH=$PATH:/path/to/blender-2.93.18-linux-x64
```

Then run following command:
```bash
source ~/.bashrc
```

## Other Install

```bash
sudo apt-get install ffmpeg
```
```

## Scripts

### 01_cube.py

- Cycles renderer

![01_cube](docs/compressed/01_cube.jpg)

### 02_suzanne.py

- Directional light
- Algorithmic object placement
- Subdivision surfaces
- `TRACK_TO` constraint to achieve camera's _look-at_ behavior
- Depth of field
- Smooth shading

![02_suzanne](docs/compressed/02_suzanne.jpg)

### 03_ibl.py

- Node-tree
- Image-based lighting using an HDR image

![03_ibl](docs/compressed/03_ibl.jpg)

### 04_principled_bsdf.py

- Principled BSDF
- Denoising
- Empty object as a target

![04_principled_bsdf](docs/compressed/04_principled_bsdf.jpg)

### 05_composition.py

- Composition nodes
- Node group

![05_composition](docs/compressed/05_composition.jpg)

### 06_split_tone.py

- Split tone effect
- Checker board texture

![06_split_tone](docs/compressed/06_split_tone.jpg)

### 07_texturing.py

- Image texture

![07_texturing](docs/compressed/07_texturing.jpg)

### 08_animation.py

- Keyframing
- Motion blur

![08_animation](docs/compressed/08_animation.gif)

### 09_armature.py

- Skeletal animation
- Skinning

![09_armature](docs/compressed/09_armature.gif)

### 10_mocap.py

- Mesh creation from Python data
- BVH data import
- Texture tiling
- Camera following

![10_mocap](docs/compressed/10_mocap.gif)

### 11_mesh_visualization.py

- Wireframe
- Vertex colors
- Transparent background

![11_mesh_visualization](docs/compressed/11_mesh_visualization.jpg)

### 12_cloth.py

- Cloth modifier
- Collision modifier
- Area light

![12_cloth](docs/compressed/12_cloth.gif)

### 13_matcap.py

- MatCap (a.k.a. Lit Sphere)
- Image filtering (e.g., sharpen)
- Simple RGB background
- Node frame

![13_matcap](docs/compressed/13_matcap.jpg)

### 14_procedural_texturing.py

- Noise texture

![14_procedural_texturing](docs/compressed/14_procedural_texturing.jpg)

## License

GNU General Public License v3.0 (GPL-3.0). We have chosen this license because we respect [the philosophy of free software](https://code.blender.org/2019/06/blender-is-free-software/).
