# Contributing Guidelines

Thank you for your interest in contributing to the **Active Theory WebGL Engine: Reverse Engineering & Architectural Specification** research project, authored and maintained by **DDW-X**.

This project is dedicated to deep systems engineering analysis, low-level browser runtime optimizations, mathematical modeling, and academic dissection of high-performance WebGL/WebAudio architectures.

---

## 1. Code of Conduct & Academic Integrity

- **Original Research**: All contributions must be original academic analysis, reproducible empirical telemetry, or mathematical derivations.
- **No Malicious Use**: Contributions designed to attack, disrupt, or exploit upstream web services or client endpoints are strictly forbidden.
- **Respect for Intellectual Property**: Maintain the clear distinction between original analytical contributions (licensed under MIT / CC BY-NC 4.0) and third-party media assets (property of Active Theory LLC).

---

## 2. Architectural & Engineering Standards

Any code, telemetry script, or mathematical formulation submitted to this repository must adhere to the high-performance engineering standards identified in the Active Theory engine:

### A. Zero-Garbage-Collection (Zero-GC) Invariant
- **No Dynamic Instantiations in Render Loops**: Never allocate objects (`new Vector2`, `new Vector3`, `new Matrix4`, `{}` literals, or anonymous closures) inside `requestAnimationFrame`, tick loops, or scroll event handlers.
- **Static Scratchpads & Object Pooling**: Utilize pre-allocated static scratchpads or instances managed by `ObjectPool`.
- **TypedArrays for GPU Data**: Transfer data to graphics buffers exclusively using pre-allocated `Float32Array`, `Uint16Array`, or `Uint8Array` instances.

### B. Mathematical Formulations & Derivations
- Any new motion curve, filter sweep, or particle kinematics component must include formal LaTeX mathematical expressions (e.g., differential equations, logarithmic interpolation `logLerp`, or FFT binning equations).
- Define all terms, coordinate systems, and units explicitly.

### C. Precise Source Code Citations
- When referencing mechanisms from the compiled bundle (`assets/js/app.1780406240914.js`), provide:
  - Exact character offsets.
  - Class / singleton name.
  - Verifiable signature or code snippet.

### D. Headless CDP Telemetry Verification
- Empirical claims regarding memory, frame pacing, or draw calls should be accompanied by reproducible headless Chrome DevTools Protocol (CDP) test scripts.

---

## 3. Contribution Workflow

1. **Fork & Branch**:
   - Create a feature or topic branch from `main`:
     ```bash
     git checkout -b feature/topic-analysis-name
     ```
2. **Commit Hygiene**:
   - Write descriptive, atomic commit messages following conventional commit specifications:
     - `docs: update mathematical proof for virtual scroll damping`
     - `telemetry: add CDP benchmark script for FBO ping-pong passes`
     - `analysis: expand GPGPU particle state texture deconstruction`
3. **Pull Request Review**:
   - Open a PR against `main`.
   - Provide a clear summary of the research addition, citing specific source files and methodology.
   - All PRs are reviewed and approved by lead researcher **DDW-X**.

---

## 4. Contact & Inquiries

For questions, academic collaboration, or research discussions:
- **Lead Researcher**: DDW-X (Cybersecurity Researcher & Reverse Engineer)
- **Email**: `ml3740965@gmail.com`
