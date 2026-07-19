# 3D Lemon Keychain 🍋

A high-fidelity, 3D-printable lemon keychain model designed from scratch using **Onshape**. 
This project serves as a technical demonstration of parametric CAD modeling, organic shape generation, and mechanical preparation for Additive Manufacturing (3D Printing).

---

##  Detailed Engineering Design Workflow
The model was constructed using a precise top-down design methodology to ensure geometric continuity, aesthetic realism, and mechanical strength.

### 1. Organic Geometry: The Lemon Body
To capture a highly realistic, organic shape rather than a standard ellipsoid, a precise parametric revolve profile was developed using exact dimensions and geometric constraints:
* **The Reference System:** Created a parametric sketch on the *Front Plane*. A vertical line of **$40\text{ mm}$** was set as a **Construction Line** through the origin, acting as the global Axis of Revolution.
* **Parametric Profile Dimensions:**
  * **Main Body Conic Arc:** Defines the wide section of the lemon with a maximum radial width constraint of **$14\text{ mm}$** from the central axis.
  * **Polar Arcs (Top & Bottom Protrusions):** Designed using precise **Conic Arcs** with a **$\text{Rho}$ value of $0.5$** to simulate the natural biological nipples of the fruit.
  * **Tip Constraints:** The upper and lower tips feature precise height offsets of **$1.5\text{ mm}$**, horizontal offsets of **$3\text{ mm}$**, and internal arc radii constraints of **$2\text{ mm}$** for strict shape control.
* **Geometric Constraints:** Applied **Tangent Constraints** between the main body arc and the polar conic sections to ensure a seamless, fluid transition (**G1 Continuity**).

## 📸 Technical Drawings & CAD Workspace

Below is the dimensioned 2D sketch profile used to generate the organic lemon geometry:
<img width="505" height="496" alt="Screenshot 2026-07-19 172345" src="https://github.com/user-attachments/assets/ecc34997-7ff9-49dd-bacc-770afad767d7" />

### 2. Mechanical Integration: The Keychain Loop
A critical aspect of functional 3D prints is structural integrity. The hanging loop was designed to withstand real-world mechanical stress:
* **Plane Offset & Sketching:** A new sketch was initiated on the *Top Plane*, structurally aligned with the absolute peak of the upper protrusion.
* **Concentric Sizing:** Sketched two concentric circles with a shared center point:
  * **Inner Diameter ($6\text{ mm}$):** Sized to provide ample clearance for standard metal split-rings or ball-chain keychains.
  * **Outer Diameter ($10\text{ mm}$):** Establishes a robust $2\text{ mm}$ solid wall thickness to resist shear stress.
* **Symmetric Extrusion & Boolean Fusion:** The profile was extruded using a **Symmetric** setting with a depth of $4\text{ mm}$. Crucially, the operation was set to **Add** with the *Merge Scope* locked onto the lemon body. This executes a Boolean union, fusing the crystalline structures of both shapes into a single, uniform solid part rather than two intersecting components, eliminating weak boundary planes.

### 3. Stress Concentration Relief & Post-Processing
* **Fillet Feature Application:** Sharp internal corners act as "stress concentrators" where structural failure typically occurs. A $1\text{ mm}$ **Fillet** was applied to the boundary intersection where the loop meets the lemon body. This distributes mechanical load evenly and enhances printability by eliminating sharp $90^\circ$ overhang transitions.
* **Mesh Optimization:** The part geometry was evaluated, and the final solid model was exported using **Fine Resolution** into an **STL** mesh, minimizing chordal error for flawless slicing.

---

## 🖨️ Technical Slicing & 3D Print Settings

Optimized for Fused Deposition Modeling (FDM) printers:
* **Material:** PLA (Polylactic Acid) or PETG for excellent layer adhesion and tensile strength.
* **Infill Density:** $15\% - 20\%$ is sufficient due to the structural fillets.
* **Infill Pattern:** **Gyroid** or **Grid** (Gyroid provides uniform isotropic strength in all directions).
* **Layer Height:** $0.12\text{ mm}$ (High Detail) to $0.20\text{ mm}$ (Standard). Smaller layer heights reduce the stair-stepping effect on the curved top surfaces.
* **Orientation:** Print standing vertically (with the flat base or loop facing upwards) or sliced horizontally depending on your support preference. Minimal supports are required only underneath the horizontal bridge of the keychain loop.

---
*Designed with engineering precision using Onshape.*
