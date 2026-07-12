docs/unreal-engine/04-materials.md# Unreal Engine Materials

## Overview

Materials define the visual appearance of objects in Unreal Engine. They determine how a surface reacts to light, reflections, transparency, and textures.

Materials are created using the Material Editor, a node-based visual tool that allows developers to build complex surface shaders without writing code.

---

## Purpose

Materials are used to:

- Define object appearance
- Control lighting interactions
- Apply textures
- Create realistic or stylized surfaces
- Build visual effects

---

## Material Editor

The Material Editor is Unreal Engine's node-based environment for creating and editing materials.

Developers connect nodes to define how a surface should behave.

### Common Features

- Node-based workflow
- Real-time preview
- Parameter support
- Material Instances
- PBR workflow

---

## PBR (Physically Based Rendering)

Unreal Engine uses a Physically Based Rendering (PBR) workflow to simulate realistic materials.

### Core Material Properties

| Property | Description |
|----------|-------------|
| Base Color | Defines the surface color |
| Metallic | Controls metallic appearance |
| Roughness | Controls surface smoothness |
| Normal | Adds small surface details |
| Emissive | Makes the material emit light |
| Opacity | Controls transparency |

---

## Material Nodes

Materials are built by connecting nodes together.

Common nodes include:

- Texture Sample
- Constant
- Multiply
- Lerp (Linear Interpolation)
- Scalar Parameter
- Vector Parameter

---

## Material Instances

Material Instances allow developers to create multiple variations of a material without duplicating the original graph.

### Advantages

- Better performance
- Easy customization
- Faster workflow

Example:

One Master Material

↓

Many Material Instances

- Red Paint
- Blue Paint
- Rusty Metal
- Clean Metal

---

## Common Use Cases

Materials are commonly used for:

- Character skin
- Clothing
- Buildings
- Weapons
- Terrain
- Water
- Glass
- Vegetation

---

## Best Practices

✔ Use Material Instances whenever possible.

✔ Keep material graphs organized.

✔ Reuse parameters.

✔ Optimize expensive shader operations.

✔ Follow PBR guidelines.

---

## Common Mistakes

❌ Using too many texture samples.

❌ Creating overly complex material graphs.

❌ Ignoring optimization.

❌ Duplicating materials unnecessarily.

---

## Related Topics

- Material Editor
- Texture Assets
- PBR Workflow
- Shader Graph (Unity)
- Lighting
- Rendering

---

## Quick Quiz

### 1. Which tool is used to create materials?

- [x] Material Editor
- [ ] Blueprint Editor
- [ ] Sequencer

---

### 2. Which property controls surface smoothness?

- [ ] Base Color
- [x] Roughness
- [ ] Metallic

---

### 3. What is the purpose of Material Instances?

- [ ] Create animations
- [x] Reuse and customize materials efficiently
- [ ] Build UI widgets
