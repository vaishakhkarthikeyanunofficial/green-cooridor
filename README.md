# Smart Ambulance Green Corridor System

## Project Overview
This project describes a digital-logic-based traffic signal controller for a single four-way junction. Push buttons simulate ambulance requests from the North, East, South, and West approaches. Request latches retain requests, a priority encoder selects the highest-priority pending request, and a finite state machine (FSM) controls the traffic lights.

## Main Features
- Four ambulance-request inputs: REQ_N, REQ_E, REQ_S, and REQ_W
- Priority order specified in the design: North > East > South > West
- Normal traffic timing specified in the design: green 8 seconds, yellow 2 seconds, all-red 1 second
- Emergency green until CLEAR is pressed or the 10-second timeout occurs
- Twelve signal indicators: red, yellow, and green for each of four approaches
- Digital logic implementation using 74HC-series ICs and a 555 timer; no Arduino or microcontroller is specified

## Repository Contents
- `Documentation/Project_Initiation_Document.pdf` — project overview, scope, deliverables, risks, and project plan
- `Documentation/Tech_Stack.pdf` — main ICs, input/output blocks, power, and tools
- `Documentation/Design_Specification.pdf` — block diagram, timing parameters, FSM states, operating behavior, and test plan
- `Documentation/Component_List.pdf` — bill of materials and component notes
- `Screenshots/` — add circuit diagrams, simulation screenshots, and hardware photos here

## Suggested Screenshots
1. Overall circuit or system block diagram
2. Priority encoder or request-input section
3. FSM and timing-counter section
4. Full traffic-light output section
5. Proteus or Logisim simulation running
6. Physical prototype, if built

## Important Note
These files describe the intended design. Update this repository with simulation evidence, hardware photographs, and measured test results only when those are actually available. Verify circuit connections and component requirements against the final schematic before building.

## How to Use
Open the PDFs in `Documentation/` to understand the project design. Add screenshots to `Screenshots/` and use clear filenames, for example `system_block_diagram.png`, `fsm_simulation.png`, or `hardware_prototype.jpg`.
