# Ski Radius Calculator

![ski2](https://github.com/user-attachments/assets/97afcb26-4d3f-4dc9-a949-0d0083ea8810)

Interactive visualization of ski geometry and turn radius physics.

Standard sidecut radius ($R$) is derived from the chord length ($L$) and sidecut depth ($d$) using the circular arc approximation:

$$R = \frac{L^2}{8d}$$

Tool uses the effective contact edge ($L_{eff}$). Different rocker profiles possible via a coefficient ($F$) where $L_{eff} = L_{total} \times F$.

## Live Demo
[https://oefi.github.io/ski-radius-calculator/]

## Usage
Input parameters:
1.  **Effective Edge ($F$):** Coefficient representing snow contact (0.91-0.94 for Piste, <0.87 for Rocker).
2.  **Dimensions:** Material length ($L$) and widths ($T, W, H$).
3.  **Visualization:** Real-time canvas rendering of the sidecut arc relative to the waist width.

## Implementation Details
* **Context:** HTML5 Canvas (2D)
* **Resolution:** High-DPI / Retina scaling implemented via `devicePixelRatio` and matrix transforms.
* **Logic:** Vanilla JS (ES6). No build step, no dependencies.
* **Rendering:** `requestAnimationFrame` loop for non-blocking UI updates.

## License
MIT
