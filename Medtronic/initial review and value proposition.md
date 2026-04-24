**Executive Summary:**

University of Minnesota researchers at the Center for Magnetic Resonance Research (CMRR) requested some industry support for developing a patient specific MRI safety monitoring method for patients with INS devices. They are asking for devices, technical assistance, and custom software. The MRI team believe that supplying **devices and limited technical enablement** would be valuable and cost effective for Medtronic. We suggest **deferring firmware development and significant engineering investment** until feasibility is demonstrated with existing implantable neurostimulator (INS) capabilities.

**Proposed scope (limited enablement):** device allocation/shipping, basic configuration guidance, one technical kickoff, and limited Q&A support. **Out of scope:** custom firmware, new telemetry/hardware development, sustained engineering support.

**Background and Problem Statement:**

Active implantable medical device (AIMD) MRI safety is currently governed by **ISO 10974**, which addresses multiple interactions between AIMDs and MRI systems. One of the most restrictive and clinically relevant interactions is **RF-induced lead/electrode heating**, where electromagnetic fields couple onto the lead and can concentrate energy near the distal electrodes.

Medtronic’s MRI safety approach for this interaction currently utilizes an **ISO 10974 Tier 3 population-based method** to ensure electrode heating remains within a safe range across a broad population and scan conditions. This is implemented through MRI labeling (e.g., power/SAR limits) intended to achieve an **estimated probability of thermal injury below 1 per 1,000,000 scans**.

While this population-based approach is robust, it has two key drawbacks:

1. **Patient access and scan flexibility:** The one in one million safety factor is inherently conservative for many patients and scanning scenarios. This can restrict access or limit scan parameters more than necessary.
2. **Residual risk:** Even with conservative limits, a population-based model still implies rare scenarios where the patient may be at risk.

**Opportunity: Patient-Specific Electrode Temperature Monitoring**

A potentially better approach is **patient-specific temperature monitoring**, where electrode temperature rise is actively inferred for the individual patient during scanning. In principle, patient-specific monitoring could enable MRI labeling that is **simultaneously less restrictive and safer**, because it focuses on real-time (or near real-time) risk at the patient/device interface rather than population-level conservatism.

Recent literature suggests patient-specific temperature estimation may be feasible using the **lead impedance as a thermistor**, leveraging the observation (demonstrated in phantom experiments) that **lead/electrode impedance changes with temperature**. Because Medtronic INS devices have impedance measurement capability, there is a plausible pathway to infer temperature from impedance—pending validation in biologically relevant conditions.

The critical remaining question is whether this impedance–temperature relationship is sufficiently accurate and repeatable **in-vivo**, where perfusion, tissue heterogeneity, electrode encapsulation, and motion may materially affect the signal.

**External Request (CMRR, University of Minnesota)**

CMRR has requested Medtronic support to evaluate whether impedance-based temperature estimation observed in phantom testing holds in an **in-vivo swine model**. They requested:

- **Devices** to test (INS systems and associated components as appropriate)
- Potential access to proprietary tools (e.g., lab programmer) and/or **custom research firmware**

The MRI team reviewed the request and believes supporting via **devices and minimal additional assistance** is a cost-effective way to enable feasibility data generation. Custom firmware and significant engineering time are not justified until feasibility is established.

**Rationale for Supporting Devices + Limited Enablement**

Providing devices and limited support creates a favorable risk/benefit profile:

- **Low incremental cost:** Device support is a comparatively small financial investment relative to the value of in vivo feasibility data.
- **Leverages external funding:** NIH-subsidized animal work allows meaningful data generation without Medtronic bearing the full study cost.
- **Data value (tangible):** With appropriate agreement terms, Medtronic can obtain **raw datasets** to enable independent analysis of impedance behavior across implant configurations and scan conditions.
- **Strategic technical positioning (intangible):** Collaboration with a leading MRI research center strengthens external technical credibility and maintains engagement in a space that could influence future MRI-conditional access and monitoring approaches.
- **Evidence generation:** Peer-reviewed publications can reduce technical and regulatory uncertainty if Medtronic later considers productizing patient-specific MRI safety monitoring.

**Why We Recommend Against Firmware and Engineering Investment**

Firmware development or substantial engineering effort should be deferred for three reasons:

- **Feasibility is not yet established in vivo:** The central uncertainty is whether impedance can predict electrode temperature rise accurately and repeatably in living tissue. Investing in firmware before feasibility is demonstrated increases the risk of sunk cost.
- **System/workflow constraints are non-trivial:** Current INS operation during MRI (e.g., requirements around MRI mode) may limit the availability of impedance measurements and/or the practicality of using those measurements for real-time monitoring.
- **Telemetry and monitoring pathway constraints:** Even if impedance can be measured, streaming or communicating measurements from the magnet room to the **control room** may require additional hardware and system-level changes beyond a low-effort research support model.

|**Category**|**Option A: Provide devices + limited enablement (Recommended)**|**Option B: Provide firmware and/or significant engineering investment (Defer)**|
|---|---|---|
|Business cost|Low (device allocation, shipping, limited staff time)|High (engineering time, testing, documentation, potential cross-functional reviews)|
|Business risk|Low–moderate (scope management; expectations; standard external research considerations)|Higher (scope creep; software/firmware governance; potential downstream expectations for productization)|
|Tangible benefits (data from study)|In vivo impedance behavior and correlation to temperature proxies; raw datasets for Medtronic analysis; feasibility signal|Potentially richer datasets and prototype-like behavior, but only if feasibility is real and system constraints are solvable|
|Intangible benefits|Strengthened academic relationship; external credibility; early positioning in patient-specific monitoring concept|Similar intangible benefits, partially offset by higher internal burden and opportunity cost|
|Key dependencies / constraints|Data access and publication review handled via standard template; clear “no firmware” boundary|Additional architecture constraints (MRI mode behavior, telemetry out of MRI environment), plus governance overhead|
|Recommended decision|Approve|Revisit after in vivo feasibility results|

**Proposed Next Steps (If Approved)**

1. Confirm device list and quantity required for the swine study and align on logistics (allocation, shipping, return/disposal if applicable).
2. Define “limited enablement” support plan (kickoff + bounded Q&A) and a single technical point of contact.

3. Need to iron out the research details on how the researchers will use the INS devices, i.e. they might need to put these devices into an MRI when they are not in MRI mode. Potentially dangerous for device?

4. Ensure standard research support template covers access to **raw data** and publication review (handled outside this memo).
5. Set a feasibility decision checkpoint (e.g., after initial cohort/results) to determine whether a phase-2 engineering discussion is warranted.


