# Spiral Exponential Function Visualizer

This repository provides an interactive visualization of trajectories generated
by the **Spiral Exponential Function**, which arises as a solution of the
**Spiral Exponential Equation (SEE)** introduced in the accompanying paper.

---

## Overview

This project visualizes the motion of a complex-valued function  
**f(t) ∈ ℂ**, whose behavior is governed by the geometric relationship between
its position vector and velocity vector.

In the framework of the Spiral Exponential Equation, the key parameter is the
angle **θ** between these two vectors. By controlling this angle, one obtains a
continuous family of motions that interpolates between different exponential
and rotational behaviors.

A representative solution exhibiting this structure is

**f(t) = exp( e^(iθ) · t )**

This repository provides an interactive tool to explore and understand the
geometry of this solution directly on the complex plane.

---

## Mathematical Background

Let **f(t)** denote the position in the complex plane.

- **Position vector**  
  f(t), pointing from the origin to the current point.

- **Velocity direction**  
  Defined by a rotation of the position vector by an angle θ:  
  **f′(t) = e^(iθ) · f(t)**

- **Acceleration direction**  
  Obtained by a further rotation:  
  **f″(t) = e^(i2θ) · f(t)**

More generally, the **n-th derivative direction** follows the rule

**f⁽ⁿ⁾(t) ∝ e^(inθ) · f(t)**

which means that each successive derivative corresponds geometrically to an
additional rotation by θ.

---

## What This Visualization Shows

By varying θ continuously, the relative orientation between the position and
velocity vectors changes. As a result, the trajectory transitions smoothly
between:

- **Growth-dominated behavior** (θ near 0)
- **Rotation-dominated behavior** (θ near π/2)

This application visualizes that continuous family of motions directly in the
complex plane, making the underlying geometric structure explicit.

---

## Features

- Interactive control of the angle **θ** using a slider.
- Interactive control of time **t**, allowing the user to move along the
  trajectory from t = 0 to the current time.
- Real-time display of the trajectory **f(t)** in the complex plane.
- Visualization of the current position as a point.
- Optional vector overlays illustrating the geometric structure of derivatives:
  - Position vector
  - Velocity direction (θ)
  - Acceleration direction (2θ)
  - Jerk direction (3θ, optional)
  - Snap direction (4θ, optional)

These vectors are shown according to the geometric rule prescribed by the Spiral
Exponential Equation, rather than as raw numerical derivatives, in order to make
the rotational structure θ, 2θ, 3θ, … visually clear.

---

## Visualization Conventions

- Position vector: <span style="color:green"><strong>green</strong></span>
- Velocity vector: <span style="color:blue"><strong>blue</strong></span>
- Acceleration vector: <span style="color:red"><strong>red</strong></span>
- Jerk vector (optional): <span style="color:purple"><strong>purple</strong></span>
- Snap vector (optional): <span style="color:orange"><strong>orange</strong></span>

The legend is placed outside the plot area so that the trajectory remains
unobstructed.

---

## Requirements

- Python 3.x  
- NumPy  
- Matplotlib  

No additional dependencies are required.

---

## Related Work

This visualization accompanies the paper:

**“Spiral Exponential Equation and Its Geometric Interpretation”**

and is intended as a supplementary tool to aid geometric intuition and
interpretation of the theory presented there.

---


## License
MIT License

## Contact
Kohei Abe
ORCID: https://orcid.org/0009-0001-1126-3282
GitHub: https://github.com/KoheiAbeLab
