# Unreal Engine Sequencer

> **Difficulty:** Beginner  
> **Estimated Reading Time:** 8 minutes  
> **Prerequisites:** Basic Unreal Engine knowledge

---

# Overview

Sequencer is Unreal Engine's cinematic editing system. It allows developers to create timeline-based animations, cutscenes, camera movements, and scripted events.

Sequencer is widely used in games, films, virtual production, and architectural visualization.

---

# Purpose

Sequencer helps developers:

- Create cinematics
- Animate cameras
- Control characters
- Synchronize audio
- Trigger gameplay events
- Produce trailers

---

# Main Features

## Timeline

The Timeline controls when animations begin and end.

Developers can:

- Move keyframes
- Trim animations
- Adjust playback speed
- Preview sequences

---

## Tracks

Tracks organize animation data.

Common track types include:

- Transform Track
- Camera Track
- Animation Track
- Audio Track
- Event Track
- Visibility Track

---

## Keyframes

Keyframes define values at a specific point in time.

Examples:

- Camera position
- Rotation
- Light intensity
- Character movement

Sequencer automatically interpolates between keyframes.

---

## Camera Cuts

Camera Cuts switch between different cameras during a cinematic.

Typical examples:

- Dialogue scenes
- Action sequences
- Gameplay introductions

---

## Level Sequence

A Level Sequence stores all cinematic data.

It can include:

- Cameras
- Characters
- Audio
- Events
- Effects

---

## Event Tracks

Event Tracks execute Blueprint events during playback.

Examples:

- Open a door
- Spawn an enemy
- Play a sound
- Trigger an explosion

---

## Movie Render Queue

Movie Render Queue exports high-quality cinematics.

Supports:

- High-resolution rendering
- Anti-aliasing
- Image sequences
- Video output

---

# Typical Workflow

Create Level Sequence

↓

Add Actors

↓

Create Tracks

↓

Add Keyframes

↓

Preview Animation

↓

Render Final Video

---

# Common Use Cases

- Game cinematics
- Cutscenes
- Dialogue sequences
- Camera animations
- Gameplay introductions
- Marketing trailers

---

# Best Practices

✔ Organize tracks clearly

✔ Name cameras properly

✔ Use folders

✔ Keep sequences modular

✔ Preview animations frequently

---

# Common Mistakes

❌ Too many unnecessary keyframes

❌ Poor camera transitions

❌ Disorganized tracks

❌ Forgetting to preview the sequence

---

# Related Topics

- Animation Blueprint
- Control Rig
- Camera Actors
- Blueprint Events

---

# Quick Quiz

### 1. What is Sequencer mainly used for?

- [x] Cinematics and timeline-based animations
- [ ] Physics simulation
- [ ] Material editing

---

### 2. What defines values over time?

- [x] Keyframes
- [ ] Components
- [ ] Variables

---

### 3. Which asset stores cinematic data?

- [ ] Blueprint
- [x] Level Sequence
- [ ] Material Instance

---

## Next Topic

➡ **07 – UMG (User Interface)**
