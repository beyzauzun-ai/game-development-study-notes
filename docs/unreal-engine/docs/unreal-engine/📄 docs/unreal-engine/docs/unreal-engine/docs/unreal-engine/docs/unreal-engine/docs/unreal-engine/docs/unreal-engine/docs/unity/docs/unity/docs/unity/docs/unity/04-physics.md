# Unity Physics

> **Difficulty:** Beginner  
> **Estimated Reading Time:** 12 minutes  
> **Prerequisites:** Unity Components

**Last Updated:** July 2026

**Category:** Unity

**Tags:** Rigidbody, Collider, Physics, Collision, Trigger, FixedUpdate

---

# Overview

Unity's Physics System simulates real-world physical interactions such as gravity, collisions, forces, and motion.

The system is primarily based on **Rigidbody** and **Collider** components.

---

# Purpose

Unity Physics allows developers to:

- Simulate gravity
- Detect collisions
- Apply forces
- Create realistic movement
- Trigger gameplay events

---

# Rigidbody

A Rigidbody enables physics simulation for a GameObject.

Common Features

- Gravity
- Velocity
- Mass
- Drag
- Angular Drag

Common Uses

- Player movement
- Vehicles
- Falling objects
- Projectiles

---

# Collider

A Collider defines the physical boundaries of a GameObject.

Without a Collider, Unity cannot detect collisions.

Common Collider Types

- Box Collider
- Sphere Collider
- Capsule Collider
- Mesh Collider

---

# Trigger Colliders

A Collider becomes a Trigger when **Is Trigger** is enabled.

Trigger Colliders detect overlaps without applying physical collisions.

Examples

- Checkpoints
- Pickups
- Damage Zones
- Quest Areas

---

# Collision Detection

Unity automatically detects collisions between GameObjects.

Common Collision Methods

### OnCollisionEnter()

Called when two Colliders physically collide.

Example

```csharp
void OnCollisionEnter(Collision collision)
{
    Debug.Log("Collision detected!");
}
```

---

### OnTriggerEnter()

Called when another Collider enters a Trigger.

Example

```csharp
void OnTriggerEnter(Collider other)
{
    Debug.Log("Entered Trigger!");
}
```

---

# Physics Methods

Physics calculations should be performed inside:

```csharp
FixedUpdate()
```

Example

```csharp
void FixedUpdate()
{
    rb.AddForce(Vector3.forward * speed);
}
```

---

# Applying Forces

Unity provides several ways to move Rigidbody objects.

Common Methods

- AddForce()
- AddTorque()
- MovePosition()
- MoveRotation()

---

# Gravity

Gravity is automatically applied when:

- Rigidbody exists
- Use Gravity is enabled

---

# Collision Matrix

Unity allows developers to define which layers can collide.

Benefits

- Better performance
- Cleaner gameplay logic
- Easier collision management

---

# Best Practices

✔ Use FixedUpdate() for physics.

✔ Keep Rigidbody objects lightweight.

✔ Use Triggers for detection zones.

✔ Configure Layers properly.

✔ Avoid unnecessary Mesh Colliders.

---

# Common Mistakes

❌ Moving Rigidbody objects using Transform.

❌ Using Update() for physics.

❌ Forgetting Colliders.

❌ Too many Mesh Colliders.

---

# Related Topics

- Components
- Rigidbody
- Collider
- C# Scripting
- Character Controller

---

# Quick Quiz

### 1. Which Component enables physics simulation?

- [ ] Collider
- [x] Rigidbody
- [ ] Transform

---

### 2. Which method is recommended for physics calculations?

- [ ] Update()
- [x] FixedUpdate()
- [ ] LateUpdate()

---

### 3. Which method detects Trigger events?

- [ ] OnCollisionEnter()
- [x] OnTriggerEnter()
- [ ] OnTriggerStay()

---

### 4. Which Component detects collisions?

- [ ] Transform
- [x] Collider
- [ ] Audio Source

---

# Mini Project

## Build a Falling Cube

### Requirements

- Create a Cube
- Add a Rigidbody
- Add a Box Collider
- Detect collision with the floor
- Print a Debug.Log() message when the cube lands

### Skills Practiced

- Rigidbody
- Collider
- FixedUpdate()
- OnCollisionEnter()
