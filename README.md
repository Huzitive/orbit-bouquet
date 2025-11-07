# Orbit Bouquet — Kepler + GR Precession

**A visual and interactive physics art project** blending **Keplerian orbits** and **General Relativistic precession**, rendered in pure **HTML, CSS, and JavaScript**.
Designed and coded with aesthetics in mind — inspired by Apple’s clean gradients and Swiss-style grid composition.

---

## 🌌 Overview

**Orbit Bouquet** simulates multiple precessing orbits (like planets around a star) using the **Keplerian equation of motion**, visually extended to include **GR precession**.
It creates a dynamic, trail-based pattern of orbits — forming a colorful bouquet-like visualization with controllable parameters.

Mathematically:
[
r(\theta,t) = \frac{a(1 - e^2)}{1 + e \cos(\theta - \varpi(t))}
]
and precession evolves as:
[
\dot{\varpi} = \Omega_{\rm GR} \approx \frac{6\pi GM}{a(1 - e^2)c^2} \frac{1}{T}
]

---

## 🎨 Features

* Interactive **UI panel** to tweak:

  * Number of orbits
  * Eccentricity
  * Precession rate
  * Trail fade
  * Orbital speed
  * Scale

* **Live performance tuning**:

  * Auto adjusts render scale and quality based on FPS
  * Displays real-time performance metrics

* **Canvas interaction**:

  * Drag to rotate
  * Double-click to recenter
  * Keyboard shortcuts:

    * `Space` → Play/Pause
    * `R` → Reset
    * `↑/↓` → Adjust precession
    * `←/→` → Adjust eccentricity

* **Mathematical equations** rendered via MathJax

---

## 🧮 Controls

| Parameter        | Range       | Default | Description                 |
| ---------------- | ----------- | ------- | --------------------------- |
| Orbits           | 6 – 120     | 48      | Number of orbital paths     |
| Eccentricity (e) | 0 – 0.95    | 0.65    | Orbital shape               |
| Precession       | 0 – 0.03    | 0.008   | GR precession per orbit     |
| Trail fade       | 0.02 – 0.25 | 0.08    | Persistence of orbit trails |
| Speed            | 0.2 – 4     | 1.3     | Orbital velocity multiplier |
| Scale            | 0.4 – 1.4   | 0.95    | Orbital size                |

---

## ⚙️ Installation & Usage

1. Clone or download the repository.

   ```bash
   git clone https://github.com/<your-username>/orbit-bouquet.git
   cd orbit-bouquet
   ```

2. Open the project:

   ```bash
   open index.html
   ```

   or simply drag `index.html` into your browser.

3. Adjust parameters with the UI or keyboard shortcuts.

---

## 🧠 Physics Behind It

This simulation models **elliptical orbits** with a **gradually rotating periapsis**, simulating **relativistic precession** like that of **Mercury’s orbit** around the Sun.

* **Keplerian term** defines the basic ellipse.
* **GR correction** adds slow angular drift over time.
* The overlapping of many such ellipses forms intricate **orbital bouquets**.

---

## 🪞 Visual Aesthetics

* Dual-color gradient scheme between **cyan and magenta**
* Smooth trail blending via `globalCompositeOperation='lighter'`
* Dynamic glow and blur tuned to device performance

---

## 🧰 Technologies Used

* **HTML5 Canvas API** for graphics
* **CSS3 gradients + glassmorphism** for UI
* **JavaScript (vanilla)** for simulation logic
* **MathJax** for LaTeX-style equation rendering


---

## 🧾 License

Released under the **MIT License**.
Free to use, modify, and share with attribution.

---

**Made with ❤ by Huzaifa Ahmed Khan**

> “Mathematics is the poetry of the universe.”
