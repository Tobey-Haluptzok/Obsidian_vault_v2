tissue can act as a thermistor where impedance closely correlates to temperature. This has been shown in agar phantoms, now Yigitcan wants to try it in-vivo.


[[initial review and value proposition]]
**Executive Summary:**
University of Minnesota researchers at the Center for Magnetic Resonance Research (CMRR) requested some industry support for developing a patient specific MRI safety monitoring method for patients with INS devices. They are asking for devices, technical assistance, and custom software. The MRI team believe that supplying **devices and limited technical enablement** would be valuable and cost effective for Medtronic. We suggest **deferring firmware development and significant engineering investment** until feasibility is demonstrated with existing implantable neurostimulator (INS) capabilities.
**Proposed scope (limited enablement):** device allocation/shipping, basic configuration guidance, one technical kickoff, and limited Q&A support. **Out of scope:** custom firmware, new telemetry/hardware development, sustained engineering support.

[[ERP review comments - Round 1]]

8840 head
TMTI lab programmer communication device
Percept PC

### *what is the dataset would be beneficial for Medtronic*
The variability in heating at high temperatures.
The variability in heating across animals.
Stability of absolute impedance over multiple heating-cooling cycles
Tissue damage

Running some back of the envelope statistics/data requirements
	animal/implant environment variability (N=8-15)
	in-vivo tissue thermistor property variability (N=8-15)
	Lead model variability (N=2)
	implant tissue type (N=2-4)
	temporal stability (30-60 minutes)

1. To be efficient with our INS systems, we should use 2 leads per INS.
2. To get implant environment variability, we will need 4 animals, each with 2 leads implanted in the same tissue
3. To get tissue variability, we can use a second INS device, also with two leads, implanted into a different tissue, like the spine or muscle
4. To get lead model variability, we can use legacy and Sensight leads
5. To get temporal stability, ensure that each animal is in the scanner for 60+ minutes

Yigitcan and the vet team at UMN has experience in reusing lead and INS systems, I think we should trust this experience and use it to our advantage to reduce material costs on our side.

This results in them asking for 2 INS devices, then recommend requesting 4 backups.
**(Total 6 INS devices)**
For the leads, we want to use both legacy and Sensight to get some variability data. For each animal, have one INS utilize legacy and one INS utilize Sensight. This results in 2 sensight leads, 1 x  90cm ext, 1 x 40cm extension. Then for backups, I'd say 2 of each system. 
**(Total 6 Sensight leads, 3 x 90cm SS extensions, 3 x 40cm SS extensions, 6 legacy leads, 3x90cm legacy extensions, 3x40cm legacy extensions)**

They need a drill to be able to do implants
**(1 x Midas Rex MR8 high-speed drill system)**



### *what is the dataset would be beneficial for UMN*
The variability in heating at high temperatures.
Stability of absolute impedance over multiple heating-cooling cycles
Tissue damage



