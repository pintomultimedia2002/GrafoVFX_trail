# Visual Effects (VFX) Simulation & Shader Graph in Unity

[![Leer en Español](https://img.shields.io/badge/Leer_en-Español-red?style=for-the-badge&logo=none)](README.md)

![Project Status](https://img.shields.io/badge/Status-Finished-green)
![Unity Version](https://img.shields.io/badge/Unity-2022.3.6f1-black?logo=unity)
![Pipeline](https://img.shields.io/badge/Render_Pipeline-URP-blue)

Academic project developed for the **Simulation (Semester 2023-2)** course. This repository hosts a technical demonstration on implementing advanced visual effects using **Shader Graph** and Unity's **Trail Renderer** system.

## 📖 Description

The main objective of this project is to explore and demonstrate the capability of real-time shader manipulation within the Unity environment. It focuses on creating dynamic visual effects, specifically trails with animated textures and dissolve effects, applicable to video games or interactive simulations.

The project makes extensive use of the **Universal Render Pipeline (URP)** to ensure optimal performance and graphical fidelity.

### 📺 Video Demo

You can watch the final result and a breakdown of how it works at the following link:

[![Watch on YouTube](https://img.shields.io/badge/YouTube-Watch_Final_Video-red?style=for-the-badge&logo=youtube)](https://youtu.be/5utf8zOruPo)

## 🚀 Technical Features

- **Custom Shader Graph:** Implementation of a complex shader (`primer_shader.shadergraph`) including:
  - **Dissolve** control (`DisolveScale`, `DesolveSpeed`) for organic disappearance effects.
  - **UV** manipulation and texture scrolling (`MainTexSpeed`) to simulate fluid movement.
  - Noise integration (Simple Noise) for natural variations in the effect.
- **Trail Renderer System:** Trail configuration in the scene (`SampleScene.unity`) that uses instantiated shader materials to generate visual tails following object movement.
- **URP Configuration:** High-fidelity rendering settings (`URP-HighFidelity`) supporting post-processing (Bloom, Vignette, Tonemapping).

## 🛠️ Technologies Used

- **Engine:** Unity 2022.3.6f1
- **Render Pipeline:** Universal Render Pipeline (URP) 14.0.8
- **Tools:** Unity Shader Graph, Core RP Library.
- **Language:** C# (for control scripts and tutorials).

## 📂 Project Structure

```text
├── Assets/
│   ├── Scenes/             # Sample Scene (SampleScene)
│   ├── Settings/           # URP Configuration Profiles and Render Data
│   ├── Shaders_David/      # Shader Graphs (.shadergraph) and Materials (.mat)
│   └── TutorialInfo/       # Scripts and informational resources
├── ProjectSettings/        # Global project settings (Tags, Physics, Quality)
└── Packages/               # Dependency manifest (URP, Visual Scripting, etc.)
```

## ⚙️ Installation & Usage

1. **Prerequisites:** Install **Unity Hub** and version **2022.3.6f1** (or a compatible newer version).
2. **Clone the repository:**

   ```
   git clone https://github.com/pintomultimedia2002/GrafoVFX_trail.git
   ```

3. **Open the Project:**

   - Add the cloned folder to Unity Hub.
   - Open the project (Unity will automatically import assets and compile shaders).

4. **Run:**

   - Open the scene `Assets/Scenes/SampleScene.unity`.
   - Press the **Play** button to visualize the simulation in real-time.

## ✒️ Author

**David Pinto** - Ingeniero Multimedia.

- [GitHub](https://github.com/pintomultimedia2002)
- [LinkedIn](https://www.linkedin.com/in/pinto-gomez-david/)

---

_Project developed for educational purposes for the Simulation course._
