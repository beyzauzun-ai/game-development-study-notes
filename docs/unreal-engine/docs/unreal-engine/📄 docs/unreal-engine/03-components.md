# Unreal Engine Components

## Overview

Components are reusable building blocks that define the functionality and behavior of an Actor.

Instead of writing everything inside a single Actor, Unreal Engine uses Components to create modular and maintainable game objects.

---

## Purpose

Components help developers:

- Build modular Actors
- Reuse functionality
- Improve project organization
- Simplify maintenance

---

## What is an Actor?

An Actor is any object that can be placed inside a level.

Examples include:

- Characters
- Cameras
- Lights
- Static Meshes
- Interactive Objects

Actors become functional by attaching Components.

---

## Common Components

### Scene Component

The Scene Component stores an object's transform.

Responsibilities:

- Position
- Rotation
- Scale

It also serves as the parent for other Components.

---

### Static Mesh Component

Displays a static 3D model.

Examples:

- Buildings
- Trees
- Furniture
- Environment Props

---

### Skeletal Mesh Component

Displays animated 3D models.

Examples:

- Characters
- Animals
- Animated Creatures

---

### Character Movement Component

Controls character movement.

Supports:

- Walking
- Running
- Jumping
- Gravity

---

### Camera Component

Represents the player's camera.

Can be used for:

- First Person
- Third Person
- Cinematics

---

### Audio Component

Plays sounds attached to an Actor.

Examples:

- Footsteps
- Ambient Audio
- Music
- Voice

---

### Particle System Component

Creates visual effects.

Examples:

- Fire
- Smoke
- Sparks
- Explosions

---

### Light Components

Used to illuminate the environment.

Examples:

- Directional Light
- Point Light
- Spot Light
- Rect Light

---

## Component Hierarchy

A Component can have child Components.

Example

Character

└── Capsule Component

  ├── Skeletal Mesh

  ├── Camera

  └── Spring Arm

---

## Best Practices

✔ Keep Components focused on one responsibility.

✔ Reuse Components whenever possible.

✔ Organize Component hierarchy clearly.

✔ Avoid unnecessary Components.

---

## Common Mistakes

❌ Adding too many Components to a single Actor.

❌ Ignoring Component hierarchy.

❌ Mixing unrelated responsibilities.

---

## Related Topics

- Blueprints
- Actor Classes
- Character Movement
- Animation Blueprint
