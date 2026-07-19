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

### Technical Drawings & CAD Workspace

Below is the dimensioned 2D sketch :

<img width="505" height="496" alt="Screenshot 2026-07-19 172345" src="https://github.com/user-attachments/assets/ecc34997-7ff9-49dd-bacc-770afad767d7" />

### 2. Designing the Keychain Loop & Attached Leaf Geometry
To complete the keychain assembly with structural functionality and organic aesthetics, a mechanical loop, connecting stem, and leaf were integrated into a specialized sketch:

* **The Keychain Loop (The Hole):** 
  * Initiated a circle centralized near the top tip of the lemon body to act as the primary clearance hole for the split-ring.
  * Used precise vertical and horizontal alignment constraints relative to the main axis of the lemon to ensure optimal structural placement.
* **The Connecting Stem:**
  * Sketched a smooth, organic curved guide line extending upwards from the top protrusion using arc tools to simulate a natural plant stem.
  * Extended a vertical construction reference line to control the height and stability of the leaf's attachment point.
* **The Leaf Profile:**
  * Constructed a closed leaf envelope using symmetrical upper and lower arcs meeting at a defined sharp tip.
  * Added a central dividing line inside the leaf profile to represent the natural leaf vein and to stabilize the geometric parameters.
* **Extrusion & Boolean Fusion:** 
  * Extruded the mechanical loop and the leaf profile concurrently to create uniform solid thickness.
  * Applied an **Add** operation to executing a Boolean fusion, seamlessly unifying the loop, stem, leaf, and lemon body into a single, high-strength component ready for physical loading.

### Technical Drawings & CAD Workspace

Below is the dimensioned 2D sketch :

<img width="743" height="460" alt="Screenshot 2026-07-19 173413" src="https://github.com/user-attachments/assets/052cb169-abd0-40fc-9e77-e072667c9cc2" />



### 3. The Final Model & Aesthetic Result

The final 3D render presents a stylized, high-quality, and modern look of the lemon keychain, blending organic shapes with smooth flat-face features for optimized printing:

* **Sleek Flat-Faceted Design:** The main body features flat parallel faces with beautifully swept organic curved profiles, giving it a modern minimalist look while providing an excellent flat surface for optimal 3D printing bed adhesion.
* **Functional Integrated Features:** 
  * The top section displays the completed mechanical clearance hole, seamlessly positioned within the upper protrusion.
  * The bottom protrusion includes a detailed concentric inner circle definition, emphasizing the natural geometry of the fruit.
* **Organic Plant Extensions:** The upper stem and leaf profiles remain visibly integrated with the main solid body, adding a dynamic, natural contrast to the geometric lines of the keychain.
* **Production-Ready Geometry:** The uniform thickness and lack of complex overhangs make this model highly optimized for clean, support-free or minimal-support manufacturing across various FDM 3D printers.

### Technical Drawings & CAD Workspace

Below is the dimensioned 2D sketch :

<img width="977" height="640" alt="Screenshot 2026-07-19 175134" src="https://github.com/user-attachments/assets/91f0e7a9-c195-4a12-a869-bfb83d4e1e60" />


---


