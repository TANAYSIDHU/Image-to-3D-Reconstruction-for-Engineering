# Single-View Image-to-3D Reconstruction for Engineering Applications
This repository presents an end-to-end implementation of a single-image to 3D reconstruction pipeline using the TripoSR framework. The project focuses on geometry-first modeling to generate CAD-compatible 3D meshes suitable for mechanical engineering, prosthetics, and manufacturing workflows. The implementation emphasizes reproducibility, stability, and practical engineering usability over visual realism.
Traditional 3D reconstruction methods rely on multi-view data or expensive scanning equipment. This project explores whether modern AI-based single-view reconstruction can serve as a practical alternative for early-stage engineering design, reverse engineering, and prosthetic modeling.
## Key Features
- Single-image to 3D mesh reconstruction
- Geometry-first pipeline (no texture baking)
- CAD-compatible outputs (OBJ / STL)
- Reproducible research-grade execution
- Engineering-oriented evaluation
## Pipeline Overview
Input Image → Background Removal → Neural Geometry Inference → Mesh Extraction → CAD Integration
![Pipeline Diagram](docs/pipeline_diagram.png)
## Technologies Used
- Python 3.10
- PyTorch (CUDA-enabled)
- TripoSR
- ONNX Runtime
- torchmcubes
- trimesh
- Blender / Fusion 360 (post-processing)
## Engineering Applications
- Mechanical design conceptualization
- Prosthetic geometry modeling
- Reverse engineering
- Additive manufacturing preparation
## Challenges Faced
- Python version incompatibilities
- Dependency conflicts in research code
- Installation of non-PyPI geometry libraries
- CUDA and CPU execution handling
## Installation

```bash
git clone https://github.com/your-username/Single-View-3D-Reconstruction-TripoSR.git
cd Single-View-3D-Reconstruction-TripoSR
pip install -r requirements.txt

---

### 🔹 8. How to Run (CRITICAL SECTION)

```markdown
## Usage

```bash
python3.10 run.py inputs/object.jpeg \
--output-dir outputs \
--device cuda \
--no-bake-texture

Mention:
- GPU recommended
- CPU fallback supported

---

### 🔹 9. Results (Visual Proof)

```markdown
## Results
The pipeline successfully reconstructs coherent 3D geometry from a single RGB image. The generated meshes can be imported into CAD environments after minimal cleanup.




