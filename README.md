# Simulación de Efectos Visuales (VFX) y Shader Graph en Unity

[![Read in English](https://img.shields.io/badge/Read_in-English-blue?style=for-the-badge&logo=none)](README.en.md)

![Estado del Proyecto](https://img.shields.io/badge/Estado-Finalizado-green)
![Unity Version](https://img.shields.io/badge/Unity-2022.3.6f1-black?logo=unity)
![Pipeline](https://img.shields.io/badge/Render_Pipeline-URP-blue)

Proyecto académico desarrollado para la asignatura de **Simulación (Semestre 2023-2)**. Este repositorio aloja una demostración técnica sobre la implementación de efectos visuales avanzados utilizando **Shader Graph** y el sistema de **Trail Renderer** de Unity.

## 📖 Descripción

El objetivo principal de este proyecto es explorar y demostrar la capacidad de manipulación de shaders en tiempo real dentro del entorno de Unity. Se centra en la creación de efectos visuales dinámicos, específicamente estelas (trails) con texturas animadas y efectos de disolución, aplicables a videojuegos o simulaciones interactivas.

El proyecto hace uso intensivo de **Universal Render Pipeline (URP)** para garantizar un rendimiento óptimo y fidelidad gráfica.

### 📺 Demostración en Video

Puedes ver el resultado final y la explicación del funcionamiento en el siguiente enlace:

[![Ver Video en YouTube](https://img.shields.io/badge/YouTube-Ver_Video_Final-red?style=for-the-badge&logo=youtube)](https://youtu.be/5utf8zOruPo)

## 🚀 Características Técnicas

* **Shader Graph Personalizado:** Implementación de un shader complejo (`primer_shader.shadergraph`) que incluye:
  * Control de **Disolución** (`DisolveScale`, `DesolveSpeed`) para efectos de desaparición orgánica.
  * Manipulación de **UVs** y desplazamiento de texturas (`MainTexSpeed`) para simular movimiento fluido.
  * Integración de ruido (Simple Noise) para variaciones naturales en el efecto.
* **Sistema de Trail Renderer:** Configuración de estelas en la escena (`SampleScene.unity`) que utilizan materiales instanciados del shader para generar colas visuales tras el movimiento de objetos.
* **Configuración URP:** Ajustes de renderizado de alta fidelidad (`URP-HighFidelity`) con soporte para post-procesamiento (Bloom, Vignette, Tonemapping).

## 🛠️ Tecnologías Utilizadas

* **Motor:** Unity 2022.3.6f1
* **Render Pipeline:** Universal Render Pipeline (URP) 14.0.8
* **Herramientas:** Unity Shader Graph, Core RP Library.
* **Lenguaje:** C# (para scripts de control y tutoriales).

## 📂 Estructura del Proyecto

```text
├── Assets/
│   ├── Scenes/             # Escena de muestra (SampleScene)
│   ├── Settings/           # Perfiles de configuración URP y Render Data
│   ├── Shaders_David/      # Grafos de shader (.shadergraph) y Materiales (.mat)
│   └── TutorialInfo/       # Scripts y recursos informativos
├── ProjectSettings/        # Configuraciones globales del proyecto (Tags, Physics, Quality)
└── Packages/               # Manifiesto de dependencias (URP, Visual Scripting, etc.)
```

## ⚙️ Instalación y Uso

1. **Requisitos:** Tener instalado **Unity Hub** y la versión **2022.3.6f1** (o superior compatible).
2. **Clonar el repositorio:**

   ```
   git clone https://github.com/pintomultimedia2002/GrafoVFX_trail.git
   ```
3. **Abrir el Proyecto:**

   * Añade la carpeta clonada a Unity Hub.
   * Abre el proyecto (Unity importará los assets y compilará los shaders automáticamente).
4. **Ejecutar:**

   * Abre la escena `Assets/Scenes/SampleScene.unity`.
   * Presiona el botón **Play** para visualizar la simulación en tiempo real.

## ✒️ Autor

**David Pinto** - Ingeniero Multimedia.

- [GitHub](https://github.com/pintomultimedia2002)
- [LinkedIn](https://www.linkedin.com/in/pinto-gomez-david/)

---

*Proyecto desarrollado con fines educativos para la materia de Simulación.*
