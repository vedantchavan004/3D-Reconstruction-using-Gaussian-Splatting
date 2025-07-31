# 📸 3D Reconstruction from Mobile Video using Gaussian Splatting

This project demonstrates how to reconstruct and render photorealistic 3D scenes from a monocular video using [Gaussian Splatting](https://github.com/graphdeco-inria/gaussian-splatting). The input is a simple video captured on a mobile phone.

## 🔧 Pipeline Overview

1. **Input**: Monocular video recorded on a smartphone.
2. **Pose Estimation**: Camera poses and sparse point cloud extracted using COLMAP.
3. **Gaussian Splatting**: Used the official implementation to generate high-quality 3D splats.
4. **Rendering**: Real-time rendering with splat-based shading, transparency, and occlusion handling.
5. **Visualization**: Interactive viewer provided using an HTML frontend + Open3D/GL.

---

## 🎥 Input & Output

- 📹 **Input Video**: [`luffy_2.mp4`](luffy_2.mp4) – Monocular video captured on a smartphone.
- 🖼️ **Screenshot**: [`2.png`](2.png) – Sample output from Gaussian Splatting render.
- 🌐 **Live Viewer**: [Launch the 3D Viewer](luffy.html) – View the reconstructed scene.

---

## 📂 Project Structure

- `colmap_output/`: COLMAP sparse reconstruction outputs.
- `gaussian_splatting/`: Gaussian Splatting configuration, model, and output.
- `viewer/`: HTML viewer for exploring the splats or point cloud.
- `input_video/`: Your monocular recording.

---

## 🛠️ Tools & Technologies

- [COLMAP](https://colmap.github.io/) for camera pose estimation
- [Gaussian Splatting](https://github.com/graphdeco-inria/gaussian-splatting)
- Open3D for 3D visualization
- Python, PyTorch
- Rendered and hosted on WSL2 (Ubuntu 22.04)

---

## ✨ Results

- High-fidelity 3D scene representation with view-dependent effects.
- Real-time interactive rendering using splats.
- Explored mesh conversion (e.g., Poisson, Marching Cubes) and Open3D integration.

---

## 🧠 Key Learnings

- From raw mobile video to sparse camera tracking using COLMAP.
- How Gaussian Splatting differs from NeRF and traditional point clouds.
- Handling transparency, occlusion, and fine details via shaders and splat parameters.

---

