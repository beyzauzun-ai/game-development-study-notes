# Unity C# Scripting

> **Difficulty:** Beginner  
> **Estimated Reading Time:** 10 minutes  
> **Prerequisites:** Basic Unity Editor knowledge

---

# Overview

C# is the primary programming language used in Unity. It allows developers to control gameplay, manage interactions, manipulate GameObjects, and create game mechanics.

Unity scripts are attached to GameObjects as Components.

---

# Purpose

C# scripting is used to:

- Control GameObjects
- Handle player input
- Create gameplay mechanics
- Manage UI interactions
- Trigger animations
- Communicate between objects

---

# MonoBehaviour

Most Unity scripts inherit from the **MonoBehaviour** class.

Example:

```csharp
using UnityEngine;

public class PlayerController : MonoBehaviour
{

}
```

MonoBehaviour provides access to Unity's event functions.

---

# Script Lifecycle

Unity executes script methods in a specific order.

```
Awake()

↓

OnEnable()

↓

Start()

↓

Update()

↓

LateUpdate()

↓

FixedUpdate()

↓

OnDisable()

↓

OnDestroy()
```

---

# Awake()

Called before Start().

Common uses:

- Initialize variables
- Cache references
- Set default values

---

# Start()

Called once before the first frame.

Used for:

- Game initialization
- Loading data
- Setting player values

---

# Update()

Runs once every frame.

Common uses:

- Player movement
- Keyboard input
- Mouse input
- Timers

---

# FixedUpdate()

Runs at fixed time intervals.

Used for physics calculations.

Examples:

- Rigidbody movement
- Applying forces
- Physics interactions

---

# LateUpdate()

Runs after Update().

Often used for:

- Camera follow systems
- Final object adjustments

---

# Coroutines

Coroutines allow execution over time.

Start a Coroutine:

```csharp
StartCoroutine(MyCoroutine());
```

Pause execution:

```csharp
yield return new WaitForSeconds(2f);
```

---

# Debugging

Unity provides debugging tools.

Example:

```csharp
Debug.Log("Player spawned.");
```

The message appears inside the Console window.

---

# Common Methods

| Method | Purpose |
|---------|---------|
| Instantiate() | Create a new object |
| Destroy() | Remove an object |
| GetComponent() | Access Components |
| StartCoroutine() | Start Coroutine |
| Debug.Log() | Print messages |

---

# Best Practices

✔ Keep scripts small.

✔ Use descriptive names.

✔ Organize methods.

✔ Comment complex logic.

✔ Avoid duplicate code.

---

# Common Mistakes

❌ Writing everything inside Update().

❌ Ignoring FixedUpdate() for physics.

❌ Creating very large scripts.

❌ Forgetting null checks.

---

# Related Topics

- MonoBehaviour
- Components
- Physics
- GameObjects
- UI

---

# Quick Quiz

### 1. Which class do most Unity scripts inherit from?

- [x] MonoBehaviour
- [ ] GameObject
- [ ] Transform

---

### 2. Which method runs every frame?

- [ ] Start()
- [x] Update()
- [ ] Awake()

---

### 3. Which method is recommended for physics?

- [ ] Update()
- [x] FixedUpdate()
- [ ] LateUpdate()

---

### 4. Which method prints messages to the Console?

- [ ] Console.WriteLine()
- [x] Debug.Log()
- [ ] PrintText()

---

## Next Topic

➡ **03 – Unity Components**
