# SKILL LAB PRATICAL HACKATHON

## Final Project README

> **Project Weight:** 100%  
> **Team Size:** 4/3 students  
> **Project Duration:** 8 hours  
> **Total Time Available:** 32 effort-hours per team  
> **Project Type:** Playful, interactive, technology-based experience

---

# Before you begin

## Fork and rename this repository

After forking this repository, rename it using the format:

`SKILLLAB_PROR-2026-TeamName`

### Example

`SKILLLAB_PROR-2026-AuroWizards`

Do not keep the default repository name.

---

# How to use this README

This file is your team’s **working project document**.

You must keep updating it throughout the build period.  
By the final review, this README should clearly show:

- your idea,
- your planning,
- your design decisions,
- your technical process,
- your build progress,
- your testing,
- your failures and changes,
- your final outcome.

## Rules

- Fill every section.
- Do not delete headings.
- If something does not apply, write `Not applicable` and explain why.
- Add images, screenshots, sketches, links, and videos wherever useful.
- Update task status and weekly logs regularly.
- Use this file as evidence of process, not only as a final report.

---

# 1. Team Identity

## 1.1 Studio / Group Name

`HeatGuard`

## 1.2 Team Members

| Name           | Primary Role                    | Secondary Role |  Strengths Brought to the Project |
| -------------- | ------------------------------- | -------------- |  -------------------------------- |
| `Arsalan` | `[Electronics]`                      | `Coding`|            | Quick Logic | 
| `Ashish`  | `[Material Handling]`                | `Presentation`|      |Good Graphic skills |
| `Heeth`   | `[Ideation]`                         | `Documentation`|     |Conceptual Knowledge | 
| `Tanaaz`  | `[Coding]`                           | `Hardware`|          | Wiring and Connections | 

<img width="1280" height="960" alt="WhatsApp Image 2026-04-28 at 11 16 16 AM (1)" src="https://github.com/user-attachments/assets/d16adb67-2bb3-4715-80cb-cd37fd8d7546" />

## 1.3 Project Title

`"HeatSafePro"`
<img width="1920" height="1080" alt="heat safe pro jpg" src="https://github.com/user-attachments/assets/c9a48014-4ff2-4a6f-a492-0dc41d1e3c30" />




## 1.4 One-Line Pitch

`A wearable system that detects dangerous heat stress in outdoor workers and alerts supervisors before it becomes fatal.`

## 1.5 Expanded Project Idea

In 1–2 paragraphs, explain:

- what your project is,
- what kind of experience it creates,
- what technologies are involved.

**Response:**  
`Every summer in India, thousands of outdoor workers — construction labourers, road workers, and daily wage earners — collapse and die from heat stroke because nobody is monitoring them. Our solution, Heat Stress Guardian, is a two part wearable safety system designed to fix this. A DHT11 sensor embedded in a cardboard wristband continuously reads temperature and humidity, sending both values to the RP2040 Shrike Lite which calculates the Heat Index — the same formula doctors and meteorologists use to assess real danger to the human body. This matters because 38°C at 90% humidity feels like 51°C and is fatal, while 38°C at 30% humidity is manageable — a basic thermometer cannot tell the difference but our device can. When the heat index crosses a critical threshold, a buzzer alerts the worker to stop, while simultaneously a red LED and serial monitor at the supervisor station display live readings and a DANGER status so the supervisor can immediately intervene.`

---

# 2. Philosophy Fit

## 2.1 Experience, Not Social Problem

`Not Applicable`

# 3. Inspiration

## 3.1 References

List what inspired the project.

Source: https://indiaobservers.com/india-heatwave-2026-early-onset-record-heat-impact/
        https://www.downtoearth.org.in/climate-change/warm-nights-above-normal-heat-waves-across-india-in-april-june-2026-imd

What makes your project original?

**Response:**  `Most heat alert systems only measure temperature. We measure heat index — temperature combined with humidity — which is the actual medical standard for heat stroke risk. We also add RFID worker registration so the system knows who is being monitored. No existing low-cost solution combines all three of these for daily wage outdoor workers.`


---

# 4. Project Intent

## 4.1 User Journey 

Describe exactly how a user will use the project.Make it a story

**Response:** `We can think its 8am on a construction site in Mumbai. Chirag, a daily wage labourer, arrives for his shift. Before picking up his tools he walks to the supervisor station and taps his RFID card to check in. The serial monitor will print his name , and start monitoring him. 
By 1pm the temperature has climbed to 38°C and humidity is at 85%. The heat index calculated by the RP2040 crosses 42°C — the danger threshold. The buzzer at the supervisor station fires hence the red LED lights up. The serial monitor flashes DANGER — HEAT INDEX 42°C — WORKER RAJAN — FORCE REST NOW.
The supervisor looks up immediately and radios Chirag to stop work and move to shade. Chirag rests for 20 minutes till the environment cools and the system resets to green. Now He can safely go back to work.`
                                                  

---

# 5. Definition of Success

## 5.1 Definition of “Usable”



## 5.2 Minimum Usable Version

What is the smallest version of this project that still delivers the core experience?

**Response:**  


## 5.3 Stretch Features

What features are nice to have but not essential?

`RFID worker registration is a good feature that adds identity tracking to the system but is not essential to the core safety function. The primary purpose of Heat Stress Guardian is detecting dangerous heat conditions and alerting supervisors in real time so this works without RFID too.`
---

# 6. System Overview

## 6.1 Project Type

Check all that apply.

- [x] Electronics-based

- [ ] Mechanical

- [x] Sensor-based

- [ ] App-connected

- [ ] Motorized

- [ ] Sound-based

- [ ] Light-based

- [x] Screen/UI-based

- [x] Fabricated structure

- [ ] Game logic based

- [ ] Installation

- [ ] Other:

## 6.2 High-Level System Description

Explain how the system works in simple terms.

Include:

- input,
- processing,
- output,
- physical structure,
- app interaction if any.

**Response:**  `The Heat Stress Guardian is a two-part worker safety system. A worker taps their RFID card to register at the start of shift — this activates monitoring. The wristband unit continuously reads temperature and humidity via DHT11, ambient light via LDR, and heart rate via pulse sensor clipped to the finger. All readings are sent to the RP2040 Shrike Lite which calculates the heat index every few seconds. If the heat index crosses 39°C the system triggers a two-stage alert — buzzer fires, red LED lights up, and the serial monitor on the supervisor's laptop displays live readings with a DANGER status showing exactly which worker is at risk. When conditions return to safe levels the green LED lights up and the system resets automatically.`

## 6.3 Input / Output Map
<img width="884" height="475" alt="Screenshot 2026-04-28 130442" src="https://github.com/user-attachments/assets/4ecce1a6-1141-48bc-bad3-bfea4fef9319" />

---

# 7. Sketches and Visual Planning

## 7.1 Concept Sketch

Add an early sketch of the full idea.

**Insert image below:**  
`[Upload image and link here]`

<img width="1600" height="902" alt="WhatsApp Image 2026-04-28 at 2 14 56 PM" src="https://github.com/user-attachments/assets/35e10c47-7fd1-486f-a7f6-b86e93efac45" />



## 7.2 Labeled Build Sketch

Add a sketch with labels showing:

- structure,
- electronics placement,
- user touch points,
- moving parts,
- output elements.

**Insert image below:**  
`[Upload image and link here]`
<img width="1280" height="720" alt="WhatsApp Image 2026-04-28 at 1 26 30 PM" src="https://github.com/user-attachments/assets/a5e2459b-ee96-4ad2-9109-9cbc80089cf2" />


## 7.3 Approximate Dimensions

| Dimension        | Value   |
| ---------------- | ------- |
| Length           | `14 cm` |
| Width            | `3 cm` |
| Height           | `-`  |
| Estimated weight | `250 g` |

---

# 8. Electronics Planning

## 8.1 Electronics Used
| Component | Quantity | Purpose |
| ------------------------- | --------: | ------------------------------------- |
| `RP2040 Shrike Lite` | `1` | Main microcontroller |
| `DHT11` | `1` | Reads temperature and humidity |
| `RFID` | `1` | Monitoring person |
| `Buzzer` | `1` | Alerts supervisor at station |
| `Red LED` | `1` | Danger indicator at station |
| `Green LED` | `1` | Safe indicator at station |
| `Breadboard` | `1` | Circuit connections |
| `Wires` | `-` | Connecting components |
| `9V Battery` | `1` | Power supply |


## 8.2 Wiring Plan

Describe the main electrical connections.

**Response:**  
`The RP2040 Shrike Lite acts as the central controller. The DHT11 temperature and humidity sensor is connected to GP0 for digital data reading. The LDR is connected to GP26 via a voltage divider with a 10k resistor to read analog light levels. The pulse sensor signal pin connects to GP27, another ADC-capable pin, for analog heart rate reading. The PIR sensor output connects to GP1 for digital presence detection.
The RFID RC522 communicates over SPI — SCK to GP18, MOSI to GP19, MISO to GP16, CS to GP17, and RST to GP20. The buzzer positive connects to GP2. Red LED connects to GP3 and green LED to GP4, each with a 220 ohm resistor in series to limit current. All component grounds connect to a common GND rail on the breadboard. The 9V battery positive connects to the VSYS pin of the RP2040 which has onboard voltage regulation.`

## 8.3 Circuit Diagram

Insert a hand-drawn or software-made circuit diagram.

**Insert image below:**  
`[Upload image and link here]`
<img width="1600" height="902" alt="WhatsApp Image 2026-04-28 at 2 13 54 PM" src="https://github.com/user-attachments/assets/f3a28640-8dd9-4249-8917-8ac48c58c5be" />



# 9. Power Plan

| Question         | Response                                                                                                                                          |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Power source     | `9V Battery(not currently mounted here)`                                                                                                                           |
| Voltage required | `3.3V for RP2040 and all sensors and 5V for LCD`                                                                  
| Current concerns | `Major concern is that Pulse sensor and RFID RC522 running simultaneously may cause minor current spikes `                                     
| Safety concerns  | `Avoid short circuits on breadboard, ensure all GND rails are connected to common ground, do not exceed 3.3V on any GPIO pin as RP2040 is not 5V tolerant, secure all jumper wire connections to prevent loose contact during demo` |

---

# 10. Software Planning

## 10.1 Software Tools

| Tool / Platform                | Purpose                                        |
| ------------------------------ | ---------------------------------------------- |
| `[Arduino IDE]`                | `Writing and uploading C++ code to RP2040 Shrike Lite`                                |
| `[MFRC522 Library]`            | `Reading RFID card UID via RC522 module` |
| `[DHT Library]`                | `[Reading temperature and humidity from DHT11]`                      |
|                                |                                                |

## 10.2 Software Logic

Describe what the code must do.

Include:

- startup behavior,
- input handling,
- sensor reading,
- decision logic,
- output behavior,
- communication logic,
- reset behavior.

**Response:**  
`Startup behavior: The RP2040 initializes all GPIO pins for buzzer, red LED, and green LED. DHT11 and LDR begin continuous reading. RFID RC522 initializes over SPI and waits for a card tap. Serial monitor prints "Heat Stress Guardian — Ready. Waiting for worker registration."
Input handling: System waits for RFID card tap first. Once worker card is detected and ID is registered, DHT11 and LDR activate monitoring. No monitoring happens before RFID registration.
Sensor reading: DHT11 reads temperature and humidity every 2 seconds. LDR reads analog light value continuously — high value means direct sunlight, low value means shade.
Decision logic: RP2040 calculates heat index from temperature and humidity. If LDR detects direct sunlight, danger threshold is lowered by 3°C. Three states — SAFE below 27°C, WARNING between 27°C and 30°C, DANGER above 30°C.
Output behavior: SAFE → green LED on, buzzer off, serial monitor prints live readings. WARNING → red LED on as visual silent alert, buzzer off, serial monitor prints "WARNING — heat index rising." DANGER → red LED on, buzzer triggers, serial monitor prints "DANGER — WORKER [ID] — HEAT INDEX [value]°C — FORCE REST NOW."
Communication logic: All output through serial monitor at 9600 baud. Supervisor laptop displays live readings in real time. No wireless communication in current version.
Reset behavior: When heat index drops below 27°C, system resets to SAFE automatically. Green LED on, buzzer off, red LED off, serial monitor prints "SAFE — conditions normal." RFID registration persists until device is powered off.`


## 10.3 Code Flowchart

Insert a flowchart showing your code logic.

Suggested sequence:

- start,
- initialize,
- wait for input,
- read input,
- decision,
- trigger output,
- repeat or reset,
- error handling.

**Insert image below:**  
<img width="2125" height="3063" alt="heat_stress_code_flowchart" src="https://github.com/user-attachments/assets/f649e540-f550-4714-9a70-34ada0b8b37c" />





# 11. Bill of Materials

## 11.1 Full BOM

<img width="2125" height="1625" alt="bom_table" src="https://github.com/user-attachments/assets/bb53fa96-fea8-4e58-9194-caaf587acc98" />


## 11.2 Material Justification

Explain why you selected your main materials and components.

**Response:**  
`The RP2040 Shrike Lite was chosen because it is our lab's standard board and we are already familiar with it. DHT11 was selected because it measures both temperature and humidity in a single module — both values are needed to calculate heat index. LDR was added to detect direct sunlight and automatically adjust the danger threshold, making the system context-aware. RFID RC522 was chosen to add worker identity tracking, active buzzer for critical danger alert, and LEDs as visual warning indicators — all selected from lab inventory to keep total cost minimal.`


## 11.3 Items You chose

| Item                 | Why Needed               | Purchase Link | Latest Safe Date to Procure | Status       |
| -------------------- | ------------------------ | ------------- | --------------------------- | ------------ |
| `Connecting wires` | `Connect all components on breadboard`   | `Local electronics store`     | `Before build day`                | `[Received]` |
| `Cardboard`     | `Physical housing for wristband and station` | `local store` | `before build day`            | `[Received]` |


## 11.4 Budget Summary

| Budget Item           | Estimated Cost              |
| --------------------- | ---------------------------:|
| Electronics           | `[0(from lab)]`                     |
| Connecting wires    | `[120]`                     |
| Fabrication materials | `[200 ]` |
| Purchased extras      | `[0]`                       |
| Contingency           | `[0]`                     |
| **Total**             | `[320]`                     |

## 11.5 Budget Reflection

If your cost is too high, what can be simplified, removed, substituted, or shared?

**Response:**  `Our total cost of ₹320 is already very low since all electronics were available in the lab at no cost. The only expenses were connecting wires and cardboard for physical housing. If cost needed to be reduced further, the cardboard housing could be skipped entirely and components left on the breadboard for demo purposes, bringing total cost down to ₹120. The RFID module could also be removed without affecting the core heat detection functionality, simplifying the build further if needed.`

---

# 12. Planning the Work

## 12.1 Team Working Agreement

Write how your team will work together.

Include:

- how tasks are divided,
- how decisions are made,
- how progress will be checked,
- what happens if a task is delayed,
- how documentation will be maintained.

**Response:**  `Task Division:
Person 1 — Hardware lead. Responsible for all physical wiring on breadboard, component connections, and circuit testing. Ensures DHT11, LDR, and RFID are correctly connected and reading data.
Person 2 — Code lead. Responsible for writing and uploading Arduino C++ code to RP2040, debugging sensor readings, and implementing heat index calculation and alert logic.
Person 3 — Documentation lead. Responsible for continuously updating GitHub README throughout the build, uploading progress photos, and maintaining the hourly log.
Person 4 — Testing and presentation lead. Responsible for testing each feature as it is built, preparing the 8-slide presentation, scripting the 60-second video, and coordinating the final demo.`


## 12.2 Task Breakdown

| Task ID | Task | Owner | Estimated Hours | Deadline | Dependency | Status |
|---------|------|-------|-----------------|----------|------------|--------|
| T1 | Brainstorm ideas and mutually decide final concept | All 4 | 1 | End of Hour 1 | None | Done |
| T2 | Finalize component list and collect from lab | All 4 | 1 | End of Hour 1 | T1 | Done |
| T3 | Set up Arduino IDE, install libraries, write base code | Arsalan | 1 | End of Hour 3 | T1 | Done |
| T4 | Code heat index calculation, RFID, LED and buzzer logic | Arsalan| 1 | End of Hour 3 | T3 | Done |
| T5 | Wire all components on breadboard | Tanaaz | 1 | End of Hour 5 | T2 | Done |
| T6 | Upload code to RP2040 and test each sensor individually | Tanaaz + Arsalan | 1 | End of Hour 5 | T4 T5 | Done |
| T7 | Full system integration test and bug fixing | All 4 | 1 | End of Hour 7 | T6 | In Progress |
| T8 | Update GitHub README with progress photos and logs | Heeth | 1 | End of Hour 7 | None | In Progress |
| T9 | Record 60 second demo video | All 4 | 0.5 | End of Hour 8 | T7 | Pending |
| T10 | Prepare and finalize 8 slide presentation | Heeth + Ashish| 0.5 | End of Hour 8 | T7 | Pending |

## 12.3 Responsibility Split

| Area | Main Owner | Support Owner |
|------|------------|---------------|
| Concept | Heeth | Ashish |
| Electronics | Arsalan | Tanaaz |
| Coding |Arsalan| Tanaaz |
| Mechanical build | Tanaaz | Ashish |
| Testing | Ashish | Arsalan |
| Documentation |Heeth | Ashish |
---

# 13. 2 hour Milestones

## 13.1 8-hour Plan

### Bi Hour 1-2 — Plan and De-risk

Expected outcomes:

- [x] Idea finalized
- [x] Core interaction decided
- [x] Sketches made
- [x] BOM completed
- [x] Purchase needs identified
- [ ] Key uncertainty identified
- [x] Basic feasibility tested

### Bi Hour 3-4 — Build Subsystems

Expected outcomes:

- [x] Electronics tests completed
- [ ] CAD / structure planning completed
- [ ] App UI started if needed
- [x] Mechanical concept tested
- [x] Main subsystems partially working

### Bi Hour 5-6 — Integrate

Expected outcomes:

- [x] Physical body built
- [x] Electronics integrated
- [x] Code connected to hardware
- [ ] App connected if required
- [x] First playable version exists

### Bi Hour 7-8 — Refine and Finish

Expected outcomes:

- [x] Technical bugs reduced
- [x] Playtesting completed
- [x] Improvements made
- [x] Documentation completed
- [x] Final build ready

## 13.2  Update Log

| Hour | Planned Goal | What Actually Happened | What Changed | Next Steps |
|------|-------------|----------------------|--------------|------------|
| Hour 1 | Finalize idea and components | Brainstormed multiple ideas, settled on Heat Stress Guardian after discussing real heatwave deaths in Maharashtra | Switched from helmet idea to wristband heat monitoring system | Collect components from lab and start wiring |
| Hour 2 | Start wiring and code setup | Collected all components, set up Arduino IDE, installed MFRC522 and DHT libraries | RFID library setup took longer than expected | Begin sensor testing and code writing |
| Hour 3 | Write heat index code and RFID registration | Completed DHT11 reading and heat index calculation, RFID card tap working on serial monitor | Removed pulse sensor as unreliable on wristband | Connect buzzer and LED output logic |
| Hour 4 | Connect all outputs and test alerts | Warning LED and critical buzzer both successfully triggered at 30°C threshold on breadboard | Threshold lowered to 30°C for lab demo environment | Attempt full integration |
| Hour 5 | Full system integration | All sensors and outputs working on breadboard — DHT11, LDR, RFID, LED, buzzer all functional | Could not build physical enclosure due to time constraint | Document breadboard setup and test results |
| Hour 6 | Physical build | Physical wristband enclosure could not be completed — remained as breadboard prototype | End product idealised but not fabricated — core electronics fully functional | Record video of breadboard demo |
| Hour 7 | Video and presentation | Recorded demo video showing breadboard working — RFID registration, warning LED, critical buzzer all demonstrated | Video shows breadboard instead of finished product | Upload to GitHub |
| Hour 8 | Final GitHub update | README completed, code pushed, progress photos uploaded | Documented breadboard as working prototype with future scope for enclosure | Submit and present |

---

# 14. Risks and Unknowns

## 14.1 Risk Register

| Risk | Type | Likelihood | Impact | Mitigation Plan | Owner |
|------|------|------------|-----------|-----------------|-------|
| LED not turning on | Technical | High | High | Checked polarity, added 220 ohm resistor, tested GPIO pin with multimeter, resolved during build | Arsalan |
| Buzzer not producing sound | Technical | High | High | Verified active buzzer type, checked positive pin connection to GPIO, confirmed with serial monitor output first, resolved during build | Heeth |
| LCD not working | Technical | High | High | LCD could not be resolved during build time — removed from final design, replaced serial monitor as output display instead | Tanaaz |

## 14.2 Biggest Unknown Right Now

What is the single biggest uncertainty in your project at this stage?

**Response:**  `The Main problem is that we have set the threshold at a certain index so if we go to areas with wide difference in temperatures so the index may never go above the threshold result in the buzzer never ringing and no warning about critical condition.`


---

# 15. Testing 

| What Needs Testing | How You Will Test It | Success Condition |
|-------------------|---------------------|-------------------|
| DHT11 sensor reading | Read temperature and humidity values on serial monitor, compare with room thermometer | Values within ±2°C of actual room temperature |
| Heat index calculation | Check serial monitor output matches manually calculated heat index for same temp and humidity values | Serial monitor shows correct heat index value |
| LDR sunlight detection | Cover LDR with hand and expose to light alternately, check serial monitor shows light condition change | Serial monitor switches between "sunlight" and "shade" correctly |
| RFID card registration | Tap card and tag to RC522 module, check serial monitor output | Serial monitor prints worker ID and "monitoring active" within 1 second of tap |
| Warning LED trigger | Warm DHT11 with hand until heat index crosses 27°C, check red LED | Red LED turns on at WARNING threshold |
| Critical buzzer trigger | Warm DHT11 further until heat index crosses 30°C, check buzzer | Buzzer sounds at DANGER threshold and serial monitor prints DANGER alert |
| System reset | Remove heat source, allow DHT11 to cool, check outputs | Red LED turns off, green LED turns on, buzzer stops, serial monitor prints SAFE |
| Full system flow | Tap RFID card, warm sensor, trigger warning then danger, remove heat source | Complete flow works end to end without any manual reset |

## 15.2 Testing and Debugging Log

| Date | Problem Found | Type | What You Tried | Result | Next Action |
|------|--------------|------|----------------|--------|-------------|
| 28th April | LCD not initializing or displaying any output | Hardware | Checked I2C address, verified wiring, tried reinitializing in code | Could not resolve within time — LCD removed from design | Switched to serial monitor as output display |
| 28th April | Buzzer not producing sound | Hardware | Checked polarity, verified GPIO pin in code, swapped to different buzzer | Resolved — active buzzer connected correctly to GP2 | Proceeded with working buzzer |
| 28th April | Red LED not glowing | Hardware | Checked polarity, added 220 ohm resistor, tested different GPIO pin | Resolved — LED was connected in reverse, flipped and worked | Proceeded with working LED |

## 15.3 Playtesting Notes

| Tester | What They Did | What Confused Them | What They Enjoyed | What You Will Change |
|--------|--------------|-------------------|-------------------|---------------------|
| Ashish | Tapped RFID card and warmed DHT11 with hand to trigger alert | Was unsure how close to hold RFID card to module for registration | Liked seeing instant serial monitor response when card was tapped | Make RFID detection range clearer with a marker on the cardboard housing |
| Tanaaz | Tested full flow from RFID tap to buzzer trigger | Could not tell difference between WARNING and DANGER state visually | Liked that buzzer and LED triggered together at danger threshold | Add a second LED or different blink pattern to distinguish WARNING from DANGER |


---

# 16. Build Documentation

## 16.1 Fabrication Process

Describe how the project was physically made.

Include:

- cutting,
- 3D printing,
- assembly,
- fastening,
- wiring,
- finishing,
- revisions.

**Response:**  
`The fabrication process for Heat Stress Guardian was kept simple and practical given the 8-hour time constraint of the build session.
Design: No CAD software was used. The system was planned on paper with a rough sketch showing component placement on the breadboard and connection layout before wiring began.
Assembly: All components were assembled directly on a full-size breadboard. The RP2040 Shrike Lite was seated centrally, with DHT11, LDR, and RFID RC522 placed around it with jumper wires routed cleanly to avoid cross-connections. Buzzer and LEDs were placed on the outer edge for easy visibility during demo.
Wiring: Male to male and male to female jumper wires were used throughout. All ground connections were routed to a common GND rail on the breadboard. Power was supplied via 9V battery connected to the VSYS pin.
Finishing: No physical enclosure was completed within the build time. The breadboard assembly was left open as a working prototype. Components were labelled with small paper tags for clarity during demo and presentation.
Revisions: Three major revisions were made during the build — LCD was removed after failing to initialize and replaced with serial monitor output, buzzer polarity was corrected after it failed to sound, and red LED was reversed after initial incorrect orientation prevented it from glowing. All three issues were identified and resolved during the testing phase.`

## 16.2 Build Photos

Add photos throughout the project.

Suggested images:

- early sketch,
- prototype,
- electronics testing,
- mechanism test,
- app screenshot,
- final build.
<img width="1280" height="721" alt="WhatsApp Image 2026-04-28 at 3 36 46 PM" src="https://github.com/user-attachments/assets/9880e678-757e-4797-84c3-fcd30935c2f3" />






# 17. Final Outcome

## 17.1 Final Description

Describe the final version of your project.

**Response:**  
`The final version of Heat Stress Guardian is a breadboard-based worker safety monitoring system that successfully demonstrates the core concept of real-time heat stress detection. The system works as follows — a worker taps an RFID card to the RC522 module to register their identity, activating the monitoring system. The DHT11 sensor continuously reads temperature and humidity, from which the RP2040 Shrike Lite calculates the heat index every 2 seconds. The LDR detects whether the worker is in direct sunlight and automatically lowers the danger threshold by 3°C to account for solar radiation. When heat index crosses 27°C a warning state is triggered with the red LED as a silent visual alert. When heat index crosses 30°C the system enters full danger mode — the buzzer sounds and the serial monitor displays "DANGER — WORKER [ID] — HEAT INDEX [value]°C — FORCE REST NOW" for the supervisor to see. When conditions return to safe levels the system automatically resets, green LED turns on, and monitoring continues.

The physical product was not completed within the 8-hour session and remains as a fully functional breadboard prototype. All core features — RFID registration, heat index calculation, sunlight detection, warning LED, and critical buzzer — were successfully demonstrated. The system proves the concept works and is ready for the next stage of development which would involve a compact PCB, wireless transmission, and a wearable enclosure for actual field deployment.`


## 17.2 What Works Well
`RFID card tap successfully registers worker and activates monitoring
DHT11 reads temperature and humidity accurately
Heat index calculation works correctly and updates every 2 seconds
Warning red LED triggers at 27°C heat index
Critical buzzer triggers at 30°C heat index
Serial monitor displays live readings clearly for supervisor
System resets automatically when conditions return to safe`



## 17.3 What Still Needs Improvement
`Physical wearable enclosure not built — currently breadboard only
LCD display could not be made to work — serial monitor used instead
No wireless communication between wristband and supervisor station yet
Pulse sensor was planned but dropped due to reliability issues
Single worker monitoring only — no multi-worker support yet
Needs real field testing in actual outdoor heat conditions`


## 17.4 What Changed From the Original Plan

How did the project change from the initial idea?

**Response:**  
`We originally planned a fully wearable wristband with LCD display, pulse sensor, and a separate wireless supervisor station. During the build we removed the pulse sensor because it cannot give reliable readings on a moving wrist, the LCD was dropped after it failed to initialize, and the wireless communication was removed due to time constraints. The final system uses serial monitor instead of LCD and remains on a breadboard instead of a wearable enclosure. The core idea and all main sensors stayed the same — only the output method and physical form changed.`


---

# 18. Reflection

## 18.1 Team Reflection

What did your team do well?  
What slowed you down?  
How well did you manage time, tasks, and responsibilities?

**Response:** ` Our team did well in quickly agreeing on a real social problem and making around it. We divided work clearly from the start — hardware, coding, documentation, and testing were each owned by specific people which kept things moving. We successfully got all core features working on the breadboard within the build time. What slowed us down was the LCD issue which cost us more than half an hour of debugging before we decided to drop it entirely. Setting up the RFID library also took longer than expected.`


## 18.2 Technical Reflection

What did you learn about:

- electronics,
- coding,
- mechanisms,
- fabrication,
- integration?

**Response:**  `For electronics, we learned to work with new sensors and modules like the RFID RC522 and DHT11 for the first time, and understood how small wiring mistakes like reversed LED polarity or wrong buzzer pin can waste significant debugging time on a breadboard.
For coding, we learned how to calculate heat index mathematically in C++ using two sensor inputs together, and how to structure code with multiple states — SAFE, WARNING, and DANGER — rather than just a simple on/off trigger.
For mechanisms, we learned that not every planned feature survives contact with reality — the pulse sensor and LCD both had to be dropped when they did not work as expected, and knowing when to cut a feature is as important as knowing how to build one.`


## 18.3 Design Reflection

What did you learn about:

- designing ,
- delight,
- clarity,
- physical interaction,
- understanding,
- iteration?

**Response:**  

`For designing, we learned that starting with a real problem — outdoor worker heat deaths — gave our design clear direction from the beginning. Every component choice had a reason behind it rather than being added randomly.

For delight, the moment the buzzer triggered and serial monitor flashed DANGER when we warmed the DHT11 with our hand was genuinely satisfying. It made the system feel real and responsive rather than just a circuit on a board.

For clarity, we learned that a system with three clear states — SAFE, WARNING, and DANGER — is far easier for a user to understand than a system with complex outputs. The green LED, red LED, and buzzer each communicate one thing instantly without needing any explanation.

For physical interaction, the RFID tap to register a worker was the most engaging part of the demo. It gave the system a clear starting point and made it feel like a real product rather than just a sensor reading numbers.

For understanding, building this project gave us a much deeper understanding of how heat index works medically and why humidity matters as much as temperature — something we would never have learned from a textbook alone.

For iteration, we went through at least three major changes during the build — dropping the pulse sensor, removing the LCD, and lowering the threshold from 39°C to 30°C. Each change made the system simpler and more reliable, and we learned that iteration is not failure but a necessary part of building anything real.`


## 18.4 If You Had One More hour

What would you improve next?

**Response:**  


We would build the physical cardboard enclosure — a wristband unit housing the DHT11 and LDR, and a separate supervisor station box housing the buzzer and LEDs. The electronics are fully working on the breadboard so the only thing missing is the physical form. One more hour would have been enough to cut, fold, and assemble the cardboard housing and make the project look like a real wearable product instead of a breadboard prototype. That single change would have made the demo significantly more convincing and visually impressive for the judges.
` `

---

# 19. Final Submission Checklist

Before submission, confirm that:

- [x] Team details are complete
- [x] Project description is complete
- [x] Inspiration sources are included
- [x] Sketches are added
- [x] BOM is complete
- [x] Purchase list is complete
- [x] Budget summary is complete
- [x] Mechanical planning is documented if applicable
- [x] App planning is documented if applicable
- [x] Code flowchart is added
- [x] Task breakdown is complete
- [x] Weekly logs are updated
- [x] Risk register is complete
- [x] Testing log is updated
- [x] Playtesting notes are included
- [x] Build photos are included
- [x] Final reflection is written


---


---


