# Unity Animation System

> **Difficulty:** Beginner  
> **Estimated Reading Time:** 12 minutes  
> **Prerequisites:** Unity Components, Unity Physics

**Last Updated:** July 2026

**Category:** Unity

**Tags:** Animation, Animator, Animation Controller, State Machine, Blend Tree

---

# Overview

Unity's Animation System enables developers to create dynamic and responsive character animations. It provides tools for controlling movement, blending animations, and managing animation transitions.

Animations are controlled using the **Animator** component and an **Animator Controller**.

---

# Learning Objectives

After completing this document, you should be able to:

- Understand Unity's animation workflow
- Configure an Animator Controller
- Create animation transitions
- Use Blend Trees
- Control animations through scripts

---

# Animation Workflow

The typical animation workflow is:

Model

↓

Rig

↓

Animation Clips

↓

Animator Controller

↓

Animator Component

↓

GameObject

---

# Animator Component

The **Animator** component plays animations on a GameObject.

Responsibilities:

- Play animations
- Blend animations
- Switch animation states
- Control transitions

---

# Animation Clips

Animation Clips store movement data.

Examples:

- Idle
- Walk
- Run
- Jump
- Attack
- Die

Multiple clips can be managed by one Animator Controller.

---

# Animator Controller

The Animator Controller defines how animations transition from one state to another.

Examples:

Idle

↓

Walk

↓

Run

↓

Jump

↓

Land

---

# State Machine

A State Machine controls which animation is currently active.

Each state represents an animation.

Transitions define when Unity changes from one animation to another.

---

# Parameters

Animator Controllers use Parameters to control transitions.

Common Parameter Types:

- Bool
- Float
- Integer
- Trigger

Example:

Speed > 0

↓

Walk

Speed > 5

↓

Run

---

# Blend Trees

Blend Trees smoothly blend multiple animations.

Common Uses:

- Walk ↔ Run
- Walk ↔ Sprint
- Aim Left ↔ Aim Right

Benefits:

✔ Smooth movement

✔ Better realism

✔ Easier animation management

---

# Animation Events

Animation Events call functions during an animation.

Examples:

- Play Footstep Sound
- Spawn Particle Effect
- Deal Damage
- Play Voice Line

---

# Root Motion

Root Motion moves the GameObject using animation data.

Advantages:

- Natural movement
- Better synchronization
- Realistic attacks

---

# Animation Scripting

Animations can be controlled through C#.

Example:

```csharp
Animator animator;

void Start()
{
    animator = GetComponent<Animator>();
}

void Update()
{
    animator.SetFloat("Speed", 5f);
}
```

---

# Best Practices

✔ Use Blend Trees for locomotion.

✔ Keep State Machines simple.

✔ Reuse animation clips.

✔ Organize Animator Controllers.

✔ Use meaningful parameter names.

---

# Common Mistakes

❌ Creating complex State Machines.

❌ Too many animation parameters.

❌ Duplicating animation clips.

❌ Ignoring Root Motion settings.

---

# Related Topics

- Components
- Physics
- C# Scripting
- Audio
- Particle System

---

# Quick Quiz

### 1. Which component plays animations?

- [ ] Rigidbody
- [x] Animator
- [ ] Audio Source

---

### 2. Which asset controls animation transitions?

- [ ] Animation Clip
- [x] Animator Controller
- [ ] Canvas

---

### 3. Which feature blends animations smoothly?

- [ ] Timeline
- [x] Blend Tree
- [ ] Rigidbody

---

### 4. Which parameter type is commonly used for attacks?

- [ ] Float
- [ ] Integer
- [x] Trigger

---

# Mini Project

## Build a Character Animation Controller

### Requirements

Create:

- Idle Animation
- Walk Animation
- Run Animation
- Jump Animation

Configure:

- Animator Controller
- State Machine
- Blend Tree

Add:

- Speed Parameter
- Jump Trigger

### Skills Practiced

- Animator
- Animator Controller
- Blend Tree
- State Machine
- Animation Parameters

---

# Further Reading

- Unity Animator
- Animation Controller
- Blend Trees
- Root Motion
