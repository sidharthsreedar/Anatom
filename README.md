Project Axis

Welcome to Project Axis!

This is an open source, in progress anatomy guide that allows the visualization of medical elements and diagnoses.

This is completely free, and allows learners to come together to understand the human body in its complexity.

Enjoy!



<img width="242" height="554" alt="Screenshot 2026-06-15 122731" src="https://github.com/user-attachments/assets/3ee74ea4-5e76-4a85-9dce-446a5bd457b3" />


Features

Imaging Modes
Drag the slider at the bottom of the viewer to transition between three medical imaging simulations:

X-Ray — greyscale wireframe skeleton with ghost-silhouette soft tissue. Nerves, arteries, and veins show in their respective colors through the body.
CT (Computed Tomography) — Hounsfield-accurate greyscale. Bone renders bright white with 3D depth shading, muscle as mid-grey, fat dark, cartilage and tendons at their correct densities. Vessels and nerves color-coded throughout.
MRI (Magnetic Resonance Imaging) — false-color T1-weighted segmentation. Each muscle compartment is mapped to its anatomical color group (anterior thigh, posterior thigh, medial, gluteal, anterior leg, lateral leg, posterior leg, foot intrinsics). Bone appears as a dark signal void, fat as bright cream, nerves as bright yellow-white.

Nervous System Tab

Divided into Central Nervous System (CNS) and Peripheral Nervous System (PNS) sections.
Full lower limb nerve tree: Lumbar Plexus (L1–L4) and Sacral Plexus (L4–S3) with all named branches.
Click any nerve to trace its territory — animated cascade highlights the selected nerve and all its branches in sequence.
Ctrl + Click to multiselect multiple nerves simultaneously.
Info panel shows spinal root, territory, and full path.

Vessels Tab

Complete lower limb arterial tree from the femoral artery down to the plantar arch and dorsal foot arteries.
Complete venous system including deep veins, the great and small saphenous superficial system, perforating veins (Boyd's, Cockett's, Dodd's), and the full plantar venous network.
Arteries shown in red, veins in blue throughout all imaging modes.
Click any vessel in the sidebar or directly on the 3D model to select and highlight it.
Ctrl + Click for multiselect.

Skeletal Muscles Tab

All 70+ muscles of the lower limb organized by anatomical compartment.
Clicking a muscle highlights it gold and flashes its origin and insertion bones in gold to show attachment sites.
Info panel displays origin, insertion, and compartment for every muscle.
Ctrl + Click to compare multiple muscles simultaneously.

Ligaments & Tendons Tab

All 104 ligaments and 15 tendons of the lower limb, searchable by name.
Includes all knee ligaments (ACL, PCL, collaterals, meniscal ligaments), ankle ligaments (talofibular, calcaneofibular, deltoid complex), foot ligaments (plantar fascia, long plantar, spring ligament, and all interosseous and tarsometatarsal ligaments), and hip ligaments.
Click any structure to highlight it on the model. Ctrl + Click for multiselect.
Search bar filters the list in real time.

Pathology Viewer

Real-time disease progression animations organized into three categories:

Vascular

Deep Vein Thrombosis (DVT) — thrombus forms in the distal deep veins and propagates proximally up the venous tree in real time. Color shifts from acute red through chronic fibrotic brown. Pulmonary embolism risk warning fires as the clot reaches the iliac/IVC level.
Peripheral Arterial Disease (PAD) — atherosclerotic plaque builds along the arteries and calcifies, with flow dimming progressively toward the foot through three stages (claudication → rest pain → critical ischaemia).
Varicose Veins / CVI — the saphenous system engorges and varicosity nodules swell along its true course, progressing from reflux through dilation to skin changes.

Musculoskeletal

ACL Tear — the anterior cruciate ligament separates into two retracting halves with a visible widening gap, and secondary meniscal involvement appears in the chronic stage.
Achilles Tendon Rupture — the calcaneal tendon splits apart and later fills with thickened scar tissue.
Lumbar Disc Herniation — a posterior bulge protrudes out of the L4–L5 and L5–S1 discs, grows during extrusion, then shrinks during resorption. The sciatic nerve lights up during nerve root compression.

Neurological

Sciatica — a bright inflammation signal travels down the sciatic nerve in real time, shifting from irritation through radiculopathy to chronic axonal change.
Common Peroneal Nerve Palsy — a compression swelling forms at the fibular neck, with anterior and lateral compartment muscle wasting in the chronic stage.

Each pathology has:

A play button for automatic progression through all stages
A scrubber to jump to any point in the timeline
Stage chips (Acute / Subacute / Chronic) with clinical timeframes
A written stage description that updates in real time

Bilateral Display

The model displays both lower limbs simultaneously — the original right leg and a mirrored left leg — sharing a single midline axial skeleton (spine, sacrum, pelvis). All selections, imaging modes, and pathology animations apply to both legs.


How to Run Locally


Clone the repository:


bash   git clone https://github.com/sidharthsreedar/Anatom.git
   cd Anatom


Start a local server (required — browsers block loading .glb files from file://):
Python:


bash   python -m http.server 8080

Then open http://localhost:8080/nerve-atlas.html

Or use VS Code + Live Server extension: right-click nerve-atlas.html → Open with Live Server.


Click Open lower-limb.glb and select the included lower-limb 4.glb file to load the model.

Created by Mohan Gadre and Sidharth Sreedar
