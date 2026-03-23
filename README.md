# 📸 BOOTH.Y2K 
> **A high-fidelity web application simulating vintage photobooth hardware.**

Built as a deep dive into **Browser APIs** and **DOM Manipulation**, BOOTH.Y2K leverages modern web technologies to recreate a nostalgic "Purikura" experience.

---

## 🛠️ Technical Architecture & Implementation

### 1. Media & Hardware Integration
- **MediaDevices API:** Implemented real-time camera streaming with a scaleX mirror transformation for user-friendly UI.
- **MediaRecorder API:** Captures 3-second "Living Strip" video buffers during the countdown sequence, synchronized with the shutter logic.

### 2. Rendering Engine (Canvas & CSS)
- **Layered Shaders:** Used CSS `mix-blend-mode: overlay` and animated keyframes to simulate high-frequency analog noise (Film Grain).
- **Canvas API:** The final output is rendered by stitching multiple `ImageData` objects into a single high-res vertical or grid layout.

### 3. State Management
- Managed complex UI transitions (Welcome → Live → Customize → Result) using a custom **Screen State** logic to handle DOM visibility without external frameworks.

---

## ✨ Core Features
- **Auto-Burst Logic:** Customizable shot counts (1-6) with programmable delay intervals.
- **Interactive Customization:** Real-time filter application using CSS filter strings (`sepia`, `saturate`, `hue-rotate`).
- **Draggable Sticker System:** Implemented event listeners for dynamic positioning of sticker elements over the canvas.

---

## 🧠 Development Methodology (AI-Augmented)
As a **1st Year CSE student**, I developed this project using an **AI-Collaborative workflow**:
- **Role:** I acted as the Software Architect/Product Manager, defining the logic flow, UI/UX design, and debugging constraints.
- **Tooling:** Leveraged **Claude (Anthropic)** for code generation, using iterative prompting to solve complex issues like video-to-blob conversion and canvas stitching.

---

## 🚀 Future Roadmap
- [ ] Implement local storage to save user "sessions."
- [ ] Optimize for mobile touch-events (PointerEvents API).
- [ ] Integrate a backend (Node.js/Firebase) for a global "Community Gallery."

---

## 🔗 Live Project
[https://boothy2k.vercel.app](https://boothy2k.vercel.app)
