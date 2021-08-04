# multipmd-dna
Multiple-path-metadynamics (MultiPMD) applied to DNA base-pairing transitions

We sample the Watson-Crick-Franklin (WCF) to Hoogsteen (HG) base-pairing transition of an A-T pair in DNA. The HG state is characterized by a 180º rotation of the A around the glycosidic bond with respect to WCF.

We use two collective variables (CVs): the base rolling angle (tBR), which describes the rotation of the A, and the base flipping angle (tBR), which describes the flipping of the A outside of the double helix.

We sample two pathways: an "inside" path in which the A rotates within the double helix, and an "outside" one in which the A flips toward the major groove and rotates before reentering the double helix. Both paths are cyclic, describing a full revolution from WCF to HG to WCF. Therefore, both the initial and final points of the path are fixed at the WCF state.

We use 12 walkers per path: walkers 0 to 8 perform standard path-metadynamics, walker 9 is an "attractor" on the HG state, and walkers 10 and 11 are "repellers" which ensure that the "inside" and "ouside' paths remain in their respective channels.
