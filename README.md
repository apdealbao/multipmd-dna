# multipmd-dna
Multiple-path-metadynamics (MultiPMD) applied to DNA base-pairing transitions

We sample the Watson-Crick-Franklin (WCF) to Hoogsteen (HG) base-pairing transition of an A-T pair in DNA. The HG state is characterized by an 180º rotation of the A around the glycosidic bond with respect to WCF.

We use two collective variables (CVs): the base rolling angle (tBR), which describes the rotation of the A, and the base flipping angle (tBR), which describes the flipping of the A outside of the double helix.

We sample two pathways, an "inside" path in which the A rotates within the double helix, and an "outside" one in which the A flips toward the major groove and rotates before reentering. Both paths are cyclic, describing a full revolution from WCF to HG to WCF. Therefore the initial and final points of the path are both fixed at the WCF state.

Walkers 0 to 8 perform standard path-metadynamics. Walker 9 is an "attractor" on the HG state. Walkers 10 and 11 are repellers which ensure that the "inside" and "ouside' paths remain in their respective channels.
