# Unreal Motion Graphics (UMG)

> **Difficulty:** Beginner  
> **Estimated Reading Time:** 8 minutes  
> **Prerequisites:** Basic Unreal Engine knowledge

---

# Overview

Unreal Motion Graphics (UMG) is Unreal Engine's user interface (UI) framework. It allows developers to create menus, HUDs, buttons, health bars, inventory systems, and other interactive interfaces.

UMG uses Widget Blueprints to design and manage UI elements without requiring extensive programming.

---

# Purpose

UMG is used to:

- Build game menus
- Create HUDs
- Display player information
- Design inventory systems
- Build settings menus
- Create interactive user interfaces

---

# Widget Blueprint

A Widget Blueprint is the primary asset used to create UI elements.

Examples:

- Main Menu
- Pause Menu
- Health Bar
- Mini Map
- Inventory
- Game Over Screen

---

# Common UI Elements

## Text

Displays information such as:

- Player Name
- Score
- Timer
- Objectives

---

## Button

Buttons allow players to interact with the interface.

Examples:

- Start Game
- Resume
- Settings
- Quit

---

## Image

Images display icons, logos, and decorative graphics.

Examples:

- Character Portrait
- Item Icon
- Game Logo

---

## Progress Bar

Progress Bars visualize values.

Examples:

- Health
- Mana
- Stamina
- Loading Progress

---

## Check Box

Used for enabling or disabling options.

Examples:

- Fullscreen
- Music
- Sound Effects

---

## Slider

Allows players to adjust values.

Examples:

- Volume
- Brightness
- Mouse Sensitivity

---

# Canvas Panel

The Canvas Panel is the root layout container.

It allows developers to freely position UI elements on the screen.

---

# HUD

HUD stands for Heads-Up Display.

Typical HUD elements include:

- Health
- Ammo
- Compass
- Objectives
- Mini Map

---

# UI Animation

Widget Blueprints support animations.

Examples:

- Fade In
- Fade Out
- Button Hover
- Menu Transition

---

# Responsive Design

Good UI should work on different screen sizes.

Recommendations:

- Use Anchors
- Use Size Boxes
- Test different resolutions
- Avoid fixed positioning

---

# Best Practices

✔ Keep interfaces simple.

✔ Group related widgets.

✔ Use consistent colors.

✔ Name widgets clearly.

✔ Optimize widget updates.

---

# Common Mistakes

❌ Creating cluttered interfaces.

❌ Ignoring screen scaling.

❌ Updating widgets every frame unnecessarily.

❌ Poor widget naming.

---

# Related Topics

- Widget Blueprint
- Blueprint
- Player Controller
- HUD
- Animation

---

# Quick Quiz

### 1. Which system is used to create UI in Unreal Engine?

- [x] UMG
- [ ] Sequencer
- [ ] Material Editor

---

### 2. Which asset is used to build UI?

- [ ] Animation Blueprint
- [x] Widget Blueprint
- [ ] Level Blueprint

---

### 3. Which widget displays player health?

- [ ] Button
- [x] Progress Bar
- [ ] Image

---

### 4. What does HUD stand for?

- [x] Heads-Up Display
- [ ] High User Display
- [ ] Human UI Device

---

## Next Topic

➡ **08 – Unreal Engine Best Practices**
