# PSE Module 2 - Filled Workbook: Serenity VR
## Systems Mapping & Root Cause
### Dissecting Problems using the Iceberg Model and Stakeholder Ecosystems

---

## Zoom in to Your Scope Area

**Scope:** The anxiety therapy delivery system in urban India - specifically the journey from a patient experiencing anxiety symptoms to receiving (or failing to receive) effective, adaptive, biofeedback-driven treatment.

---

## Identify Events (Visible Issues)

The following visible events, issues, and situations are observed within the system scope:

### Main Problem Events:
1. Patients with anxiety disorders are unable to find available mental health professionals within a reasonable timeframe (wait times of 2-8 weeks).
2. Therapy sessions follow fixed protocols (CBT, talk therapy) that do not adapt to the patient's real-time physiological state.
3. There is zero biometric monitoring during therapy - clinicians rely entirely on patient self-reporting, which is subjective and often inaccurate.
4. Patients drop out of therapy after 3-5 sessions due to high costs (Rs.500-3000/session), travel burden, and lack of perceived real-time progress.

### Trigger Events (happen just before the problem):
5. A patient experiences an acute anxiety episode or panic attack but cannot access immediate professional help.
6. A student faces exam stress, workplace pressure, or social anxiety but finds no affordable local mental health support.
7. Post-COVID mental health awareness increased, but the infrastructure did not scale proportionally.

### Effect Events (happen as a result of the problem):
8. Untreated anxiety compounds into more severe conditions (depression, substance abuse, chronic insomnia).
9. Patients resort to self-medication (over-the-counter sedatives, alcohol) without professional guidance.
10. Workplace productivity drops; absenteeism increases due to unmanaged anxiety disorders.
11. Families of patients face emotional and financial burden from managing untreated mental health conditions.

### Indirectly Connected Events:
12. Rise in mental health apps (Calm, Headspace) shows demand, but these apps lack biometric integration, clinical oversight, and adaptive therapy.
13. VR headset prices have dropped significantly (Meta Quest 3 at ~$500), making immersive therapy technologically feasible for the first time.
14. Local AI models (Llama 3, Mistral) can now run on consumer hardware, enabling personalized guidance without cloud dependency or privacy concerns.

---

## Identify Events & Patterns

### Recurring Patterns Identified:

| Pattern # | Pattern Description | Frequency | Conditions |
|-----------|-------------------|-----------|------------|
| P1 | Patients delay seeking help for weeks/months after symptom onset due to stigma and lack of awareness | Continuous | Strongest in conservative social environments and rural areas |
| P2 | Long wait times (2-8 weeks) to see a psychiatrist in urban India | Chronic | Worse during exam seasons (Mar-May) and post-pandemic periods |
| P3 | High therapy dropout rates after 3-5 sessions | Recurring per patient | Triggered by cost accumulation, travel fatigue, and lack of visible progress |
| P4 | Therapy outcomes plateau because sessions are spaced too far apart with no monitoring in between | Recurring across patients | Every therapy cycle where sessions are weekly/biweekly |
| P5 | Clinicians lack objective physiological data - rely entirely on subjective self-reports from patients | Every session | Universal across all current therapy delivery methods |
| P6 | Anxiety symptoms peak during morning commutes, work hours, and late-night screen time but therapy sessions happen at fixed, unrelated times | Daily cycle | Urban working professionals and students |
| P7 | Awareness of mental health is increasing (post-COVID), but supply of professionals and tools is stagnant | Yearly trend | Widening gap year over year since 2020 |

---

## Stakeholder Group Analysis (from Module 1)

### Stakeholder Group 1: Anxiety Patients (End Users)

**Process & Lifecycle from their perspective:**

```
Experiences anxiety symptoms (racing heart, shortness of breath, panic)
    |
    v
Denial / self-management phase (tries breathing exercises, meditation apps)
    |
    v
Symptoms worsen or become frequent -> decides to seek professional help
    |
    v
Searches online for psychiatrist/psychologist -> finds limited options
    |
    v
Books appointment -> waits 2-8 weeks
    |
    v
Attends first session (30-60 min) -> discusses symptoms verbally
    |
    v
Receives generic treatment plan (CBT exercises, possible medication)
    |
    v
Returns home -> no monitoring, no feedback between sessions
    |
    v
Tries to follow exercises on own -> lacks motivation without real-time feedback
    |
    v
Misses follow-up appointments (cost, time, travel, stigma)
    |
    v
Symptoms return / worsen -> CYCLE REPEATS or patient gives up entirely
```

**Lifecycle:** This cycle repeats every 1-3 months per patient, with each iteration increasing the probability of permanent dropout.

---

### Stakeholder Group 2: Clinicians / Therapists

**Process & Lifecycle from their perspective:**

```
Receives appointment booking (already overbooked - 15-30 patients/day)
    |
    v
Conducts 30-60 min session -> asks patient to self-report symptoms
    |
    v
Forms assessment based on SUBJECTIVE verbal input only (no physiological data)
    |
    v
Prescribes treatment plan (CBT, medication, relaxation techniques)
    |
    v
Schedules next session in 1-2 weeks -> has NO visibility into patient between sessions
    |
    v
Patient may or may not return for follow-up
    |
    v
If patient returns: reassesses based on patient's memory of past week (unreliable)
If patient doesn't return: no way to track or intervene
    |
    v
Clinician moves to next patient -> limited time per patient -> quality suffers
```

**Lifecycle:** Daily cycle, repeated for each of the 15-30 patients seen per day. Burnout risk is high.

---

### Stakeholder Group 3: Healthcare Institutions / Hospitals

**Process & Lifecycle from their perspective:**

```
Allocates budget for mental health department (typically underfunded)
    |
    v
Hires limited psychiatrists/psychologists (shortage in market)
    |
    v
Opens appointment slots -> slots fill up immediately (excess demand)
    |
    v
Long waitlists form -> patient dissatisfaction increases
    |
    v
Patients seek private practitioners or give up entirely
    |
    v
Institution cannot demonstrate treatment outcomes (no longitudinal data)
    |
    v
Difficult to justify increased mental health budget -> funding stays flat
    |
    v
CYCLE REPEATS: understaffed, overbooked, no outcome data
```

**Lifecycle:** Annual budget cycle, with the gap widening each year.

---

## Identify the System Structure

Going through the process step by step, the following structures enable/constrain the system:

| Process Step | Underlying Structure |
|-------------|---------------------|
| Patient experiences symptoms | Biological/neurological predisposition; environmental stressors (work, academics, social media) |
| Patient delays seeking help | Social stigma around mental health; lack of awareness about available treatments; cultural beliefs ("anxiety is not a real illness") |
| Long wait times to see professionals | Severe shortage: ~0.3 psychiatrists per 100,000 population; geographic concentration in metro cities; no technology-assisted triage |
| Therapy sessions are fixed-protocol | Clinical training models that emphasize standardized CBT/medication protocols; no infrastructure for real-time biometric integration |
| No monitoring between sessions | Absence of wearable biometric devices in therapy workflows; no real-time data pipeline from patient to clinician |
| Patient drops out | High cost structure (Rs.500-3000/session); no tangible progress indicators; no gamification or engagement mechanisms |
| Clinician lacks objective data | No sensor/biofeedback integration in current therapy setups; reliance on subjective patient self-reporting |
| No scalable delivery mechanism | Therapy requires physical presence; no VR/telemedicine infrastructure for immersive remote therapy |
| AI not used in therapy | Local AI inference on consumer hardware is a recent development (2023-2024); no established clinical protocols for AI-assisted therapy |

---

## Explore Mental Models

### Mental Model Analysis per Stakeholder:

| Aspect | Anxiety Patient | Clinician / Therapist | Healthcare Institution |
|--------|----------------|----------------------|----------------------|
| **Belief about therapy** | "Therapy should give me instant relief" / "If I don't feel better after 3 sessions, it's not working" | "I can only assess what the patient tells me - I trust their self-report" | "Mental health is important but not revenue-generating enough to prioritize" |
| **Expectation** | Affordable, convenient, private, and effective treatment | More patients seen per day, better tools for assessment | Measurable outcomes to justify budget allocation |
| **Assumption** | "Technology can't help with something as personal as anxiety" / "VR is just for gaming" | "Biometric data would be useful but is too complex to integrate into my workflow" | "Scaling mental health requires hiring more doctors - there's no alternative" |
| **Priority** | Immediate symptom relief; low cost; no stigma | Accurate diagnosis; manageable workload; patient retention | Cost efficiency; reputation; regulatory compliance |
| **Value** | Privacy, convenience, tangible progress tracking | Evidence-based tools, reliable data, reduced burnout | Scalability, ROI, patient satisfaction metrics |

### Common Expectations:
- All stakeholders want **better treatment outcomes**
- All stakeholders want **reduced cost and effort per interaction**
- All stakeholders want **objective, measurable data** instead of subjective assessments

### Conflicting Priorities:
- Patients want **immediate, affordable access** vs. Institutions want **cost-controlled, revenue-positive services**
- Clinicians want **more time per patient** vs. Institutions want **more patients per clinician**
- Patients want **privacy** vs. Clinicians want **continuous monitoring data**

### Shared Assumptions (that may be wrong):
- "Effective therapy MUST involve a human therapist in real-time" (VR + AI can supplement)
- "Biometric monitoring is too expensive/complex for routine therapy" (ESP32 + MAX30102 costs < Rs.500)
- "Scaling therapy = hiring more professionals" (technology can multiply reach)

---

## Iceberg Model Summary

```
============================================================
                    ICEBERG MODEL
============================================================

EVENTS (Tip - What we see):
------------------------------------------------------------
- 85-90% treatment gap for anxiety in India
- Patients waiting 2-8 weeks for appointments
- High therapy dropout after 3-5 sessions
- No real-time biometric data in therapy
- Rising anxiety prevalence (120%+ since 1990)

PATTERNS (Below surface - What keeps happening):
------------------------------------------------------------
- Consistent year-over-year widening of demand-supply gap
- Recurring patient dropout cycle every 1-3 months
- Therapy outcomes plateau due to disconnected sessions
- Daily anxiety triggers (commute, work) misaligned with
  weekly/biweekly therapy timing
- Post-COVID acceleration of mental health crisis

STRUCTURES (Deeper - What allows this):
------------------------------------------------------------
- Only 0.3 psychiatrists per 100,000 (vs WHO's 3.0)
- No biometric sensor integration in therapy workflows
- Therapy requires physical co-presence (no VR/remote)
- Fixed-protocol CBT not adaptive to real-time state
- High cost structure (Rs.500-3000/session)
- No data pipeline between patient and clinician

MENTAL MODELS (Root - Why the system is this way):
------------------------------------------------------------
- "Effective therapy must have a human therapist present"
- "Scaling = hiring more doctors (no tech alternative)"
- "Biometric monitoring is too complex for therapy"
- "VR is entertainment, not medicine"
- "Mental health stigma discourages seeking help"
- "If I don't feel better quickly, therapy doesn't work"
============================================================
```

---

## Review Your Project - Bottlenecks Identified

### 1. Key Data Bottleneck:
**No real-time physiological data flows from patient to clinician.** Therapy decisions are based entirely on subjective self-reports. The system has zero objective biometric input (heart rate, SpO2, stress indicators) during or between sessions. This means clinicians are essentially "flying blind" - making treatment decisions without the most critical data.

### 2. Key Process Bottleneck:
**Therapy delivery requires physical co-presence and follows fixed schedules.** The current process mandates in-person visits on pre-set appointments, creating a single point of failure. If a patient can't travel, can't afford it, or faces stigma, the entire therapeutic process halts. There is no mechanism for adaptive, real-time therapy delivery.

### 3. Key Human Bottleneck:
**Critical shortage of mental health professionals acts as a hard capacity limit.** With only ~0.3 psychiatrists per 100,000 population, no amount of process improvement can address the fundamental supply constraint. Each clinician is overloaded (15-30 patients/day), leading to short sessions, burnout, and quality degradation.

---

## Reviewing "How Might We" from Module 1

### How does the proposed HMW fix the bottlenecks?

| HMW Statement | Bottleneck Addressed | How It Fixes It |
|---------------|---------------------|-----------------|
| **HMW 1:** VR-based anxiety therapy at home with real-time biometric feedback | **Process Bottleneck** - Eliminates requirement for physical co-presence. Patient can receive adaptive therapy at home via VR headset. Biometric sensors provide real-time data that drives scene adaptation. |
| **HMW 2:** Local AI dynamically personalizes therapeutic guidance based on live SpO2 and pulse data | **Data Bottleneck** - Creates a continuous biometric data pipeline (MAX30102 -> ESP32 -> Backend). AI uses this data to personalize guidance in real-time. Clinicians finally have objective, physiological evidence. |
| **HMW 3:** Continuous biometric tracking with clinician dashboards and historical analytics | **Human Bottleneck** - Multiplies clinician reach by enabling remote monitoring of multiple patients simultaneously via dashboards. Reduces need for every interaction to be 1-on-1 in-person. AI handles routine adaptive sessions; clinician intervenes only when needed. |

### Which bottlenecks can be fixed with the HMW?

- **Data Bottleneck:** FULLY addressable - sensor hardware (MAX30102 + ESP32) + backend pipeline + React dashboard creates end-to-end data flow.
- **Process Bottleneck:** FULLY addressable - VR therapy at home removes physical co-presence requirement; AI + biofeedback enables adaptive sessions.
- **Human Bottleneck:** PARTIALLY addressable - technology can multiply reach of existing professionals but cannot fully replace human clinical judgment for complex cases. The system acts as a force multiplier, not a replacement.

---

## Complete the System Map (Revised from Module 1)

After Module 2 analysis, the system map is updated to include the identified bottlenecks and stakeholder interactions:

```
                        ENVIRONMENT
    +--------------------------------------------------+
    |  Social Stigma    Government Policy    Insurance  |
    |  Family Support   Pharma Industry      ISP/WiFi   |
    +--------------------------------------------------+
          |                    |                  |
          | (influences)       | (regulates)      | (enables)
          v                    v                  v
    +==========================================================+
    |              SERENITY VR SYSTEM (Scope)                   |
    |                                                          |
    |  GREEN INPUTS:                                           |
    |  -> Patient physiology (heartbeat, SpO2)                 |
    |  -> Clinician parameters                                 |
    |  -> AI model weights (Llama 3)                           |
    |  -> Power + Network                                      |
    |                                                          |
    |  +----------+  I2C  +-------+  MQTT/WS  +-----------+   |
    |  | MAX30102  |------>| ESP32 |---------->| Spring    |   |
    |  | (Sensor)  |       | (MCU) |           | Boot      |   |
    |  +----------+       +-------+           | Backend   |   |
    |       ^                                  +-----+-----+   |
    |       | worn by                           |    |    |     |
    |  +----+-----+                        +----+  +-+--+ +-+  |
    |  | Patient  |<-- Adaptive VR ---|Unity|  |React|  |AI|   |
    |  |          |     Scenes        | VR  |  |Dash |  |  |   |
    |  +----------+                   +-----+  +--+--+  +--+   |
    |                                            |              |
    |                                      +-----+------+      |
    |                                      | Clinician  |      |
    |                                      +------------+      |
    |                                                          |
    |  RED OUTPUTS:                                            |
    |  <- Reduced anxiety (desirable)                          |
    |  <- Session reports & analytics (desirable)              |
    |  <- Heat/noise/privacy risk (waste)                      |
    +==========================================================+
```

**Key Changes from Module 1 Map:**
- Added environment influences (stigma, policy, insurance)
- Clarified input/output arrows with green/red labels
- Highlighted the three bottleneck points in the data/process/human flow

---

## Module 2 Resources & Reading Links

- The Waters Center for Systems Thinking: waterscenterst.org - Interactive guides and templates for the Iceberg Model and systems mapping
- Miro Online Templates: miro.com - Free digital whiteboard templates for Iceberg Model and Ecosystem mapping
