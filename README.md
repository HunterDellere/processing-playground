# Processing Playground

A collection of creative coding experiments and generative art sketches built with **Processing (Java)**. This repository serves as a sandbox for exploring algorithmic design, visual mathematics, and object-oriented programming concepts.

## 📖 About the Project

This project represents an exploration of code as a creative medium. The scripts within this repository demonstrate various computational techniques, ranging from particle systems to noise algorithms.

While primarily focused on visual output, the codebase uses Object-Oriented Programming (OOP) principles to create modular, reusable, and scalable visual components. As it is a creative project, some structure and clarity are missing.

## 📸 Gallery

<table>
  <tr>
    <td valign="top" width="33%">
      <img src="https://github.com/user-attachments/assets/02679e7f-4b34-4f58-8d9a-42597ae2605e" alt="Sketch 1" width="100%" />
    </td> 
    <td valign="top" width="33%">
      <img src="https://github.com/user-attachments/assets/58a9f44c-8e50-4ea3-893f-d8b66a511d5f" alt="Sketch 3" width="100%" />
    </td>
    <td valign="top" width="33%">
      <img src="https://github.com/user-attachments/assets/552c9193-1225-4096-8ce6-1b947c142881" alt="Sketch 6" width="100%" />
    </td>
  </tr>
  <tr>
    <td valign="top" width="33%">
      <img src="https://github.com/user-attachments/assets/96eb66b6-b67f-4e41-b047-14296e5708cd" alt="Sketch 4" width="100%" />
    </td>
   <td valign="top" width="33%">
      <img src="https://github.com/user-attachments/assets/a8c36493-3913-46ec-ae38-ebeb4dc5fc87" alt="Sketch 2" width="100%" />
    </td>
    <td valign="top" width="33%">
      <img src="https://github.com/user-attachments/assets/274f848a-cc5b-464a-b144-c71a194ff66b" alt="Sketch 5" width="100%" />
    </td>
  </tr>
</table>


## 🚀 Technical Highlights

This repository showcases the following technical concepts:

* **Object-Oriented Design:** Encapsulation of visual elements (agents, particles, grids) into classes to manage state and behavior.
* **Algorithmic Logic:** Implementation of physics simulations, flocking behaviors, or recursive patterns.
* **Java Fundamentals:** Utilization of inheritance, polymorphism, and data structures within a creative context.
* **Generative Art:** usage of Perlin noise, trigonometry, and randomness to produce non-deterministic visuals.

## 📂 Sketch Overview

*Note: Since the scripts are creative experiments, this section helps viewers navigate the underlying concepts.*

| Script Name | Description | Key Concepts |
| :--- | :--- | :--- |
| **`s0001`** | **Flow Field Particles**<br>Generates a vector field using Perlin noise and releases particles to trace the flow. Features high-res export logic for print. | • **Flow Fields:** Using `PVector.fromAngle(noise)` to direct motion.<br>• **Particle Systems:** OOP implementation of velocity, acceleration, and force accumulation.<br>• **Spatial Mapping:** 2D grid mapping to vector arrays. |
| **`s0004`** | **Radial Growth & Decay**<br>Simulates organic, noise-driven growth radiating from a center point. Includes lifecycle management where nodes age, change mass, and die. | • **Polar-to-Cartesian:** Converting angle/radius to (x, y) coordinates.<br>• **Lifecycle Algorithms:** Logic for `age`, `growth`, and mass decay over time.<br>• **Generative Palettes:** Dynamic HSB color generation and palette arrays. |
| **`s0006`** | **3D Spherical Mesh**<br>Constructs a 3D sphere using latitude/longitude mapping and renders it as a connected vertex strip. | • **3D Rendering (P3D):** Spherical geometry logic (`x = r * sin(lat) * cos(lon)`).<br>• **Vertex Shapes:** Using `beginShape(TRIANGLE_STRIP)` for efficient mesh rendering.<br>• **Camera Control:** Integration of `PeasyCam` for interactive 3D viewing. |
| **`s0007`** | **Masked Grid Flow**<br>Initializes agents on a grid but restricts drawing to a circular area using distance checks. | • **Spatial Masking:** Conditional rendering based on distance from center.<br>• **Custom Geometry:** Custom `beginShape()` logic to draw oriented boxes.<br>• **Grid Initialization:** Nested loop instantiation. |
| **`s0008`** | **Textured Agents**<br>Agents that evolve from solid shapes into crosshatched textures as they age, with adjustable polygon fidelity. | • **Procedural Texturing:** Algorithms for "crosshatching" and end-caps.<br>• **Variable Fidelity:** Using a `fidelity` loop to draw circles as low-res polygons.<br>• **Attractors:** Implementing gravitational pull toward the center. |
| **`s0009`** | **Stippling & Triangles**<br>Focuses on rendering agents as triangle strips or pointillist fields rather than continuous lines. | • **Pointillism:** Rendering shapes via high-density point loops.<br>• **Triangle Strips:** Using `beginShape(TRIANGLE)` for geometric fills.<br>• **Palette Shuffling:** Randomized array swapping for color variation. |
| **`s0012`** | **Circle Packing & Batching**<br>A complex system that spawns agents with collision detection to prevent overlap ("packing") and automates large batch exports. | • **Collision Detection:** Bounding-box logic to prevent agent overlap (Packing).<br>• **Batch Automation:** Logic to auto-reset and save `numRenders` sequentially.<br>• **Vector Export:** PDF and SVG recording pipelines for plotters/print. |

## 🛠️ Getting Started

### Prerequisites

* **Processing IDE:** Download and install from [processing.org](https://processing.org/download/).
* **Java Development Kit (JDK):** (Optional) If you prefer running these in a standard Java environment like IntelliJ or Eclipse, you will need the Processing core library.

### Installation & Usage

1. **Clone the repository:**
```bash
git clone https://github.com/HunterDellere/processing-playground.git
```

2. **Open a sketch:**
* Navigate to the specific folder of the sketch you wish to run.
* Open the `.pde` file using the Processing IDE.

3. **Run:**
* Press the **Play** button (▶) in the top-left corner of the IDE.


## 📄 License

This project is open source and available under the [MIT License](https://tlo.mit.edu/understand-ip/exploring-mit-open-source-license-comprehensive-guide).
