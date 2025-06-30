# Syllabus


### Day 1: Introductions, Syllabus, Brief History of Robotics and Computation, Basic Math for Physics
**Learning Objectives:**
- Understand the program structure and expectations.
- Gain an overview of the history and evolution of robotics and computation.
- Review essential mathematical concepts (algebra, basic calculus) relevant to physics and robotics.

**Activities:**
- **Introductions and Syllabus (45 minutes):**
  - Instructor and student introductions.
  - Review of the course syllabus, daily schedule, learning objectives, and expectations.
  - Discussion of safety guidelines for working with electronics and robotics.

- **Brief History of Robotics and Computation (60 minutes):**
  - From ancient automatons to modern AI-driven robots.
  - Key milestones in robotics (e.g., industrial robots, Mars rovers, humanoid robots).
  - Evolution of computing: from mechanical calculators to microprocessors.
  - Discussion: How have these two fields influenced each other?

- **Basic Math for Physics and Robotics (75 minutes):**
  - Algebra Review:
    - Solving linear equations.
    - Working with exponents and logarithms for scientific notation.
    - Rearranging formulas (e.g., for Ohm's Law).
  - Introduction to Vectors:
    - What are vectors? (Magnitude and direction).
    - Basic vector operations (addition, subtraction - conceptual).
    - Relevance in robotics (e.g., robot movement, force).
  - Introduction to Calculus (30 minutes depending on prior knowledge):
    - Derivatives: Understanding rate of change (e.g., velocity from position, acceleration from velocity).
    - Integrals: Understanding accumulation (e.g., position from velocity).
    - Relate these concepts to robot motion and sensor data analysis (e.g., how a robot knows its speed or position).

---
# Challenge

# 🤖 Robotic Arm Motion Challenge

A robotic arm on a factory line moves an object along a smooth path. Its **acceleration over time** is modeled as:

```
a(t) = 4 - 0.5t   (in meters per second squared)
```

### Conditions

* The robot starts at rest:
  `v(0) = 0 m/s`
* The arm operates for `t = 0` to `t = 6` seconds.
* At the end of 6 seconds, the object is released.
* The release velocity makes a **45° angle above the horizontal**.

---

## ❓ Tasks

1. Compute the velocity function `v(t)` by integrating acceleration.
2. Calculate the magnitude of velocity at `t = 6` seconds.
3. Decompose the velocity into horizontal and vertical components.
4. Compute the work done by the applied force using the **dot product**.
5. Compute the average power used over the interval.

---

## ✅ Solutions

### 1. Integrate acceleration to get velocity

```
v(t) = ∫(4 - 0.5t) dt = 4t - 0.25t² + C
```

Using the initial condition `v(0) = 0`:

```
C = 0
=> v(t) = 4t - 0.25t²
```

---

### 2. Find velocity at `t = 6` seconds

```
v(6) = 4(6) - 0.25(6²) = 24 - 9 = 15 m/s
```

---

### 3. Decompose velocity vector at 45°

Given speed = 15 m/s and angle = 45°:

```
vx = 15 * cos(45°) ≈ 15 * 0.7071 ≈ 10.61
vy = 15 * sin(45°) ≈ 15 * 0.7071 ≈ 10.61
```

**Velocity vector:**

```
v = <10.61, 10.61> m/s
```

---



## ✅ Final Answers

| Quantity              | Value                |
| --------------------- | -------------------- |
| Velocity function     | `v(t) = 4t - 0.25t²` |
| Velocity at `t = 6 s` | `15 m/s`             |
| Velocity vector       | `<10.61, 10.61> m/s` |
