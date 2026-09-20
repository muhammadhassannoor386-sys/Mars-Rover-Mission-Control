Mars Rover Mission Control — Requirements Analysis
1. Mission: Analyze the Engineering Note
Functional Requirements (FRs)
Functional requirements describe what the system must do.

FR-01 — Send Commands
The system shall allow Mission Control to send movement commands to the rover.

FR-02 — Execute Valid Commands
The rover shall receive and execute valid commands from Mission Control.

FR-03 — Report Rover Status
The rover shall report its current position, battery level, temperature, and communication status.

### FR-4: Command Execution
The system shall accept movement commands consisting of
forward, left, and right instructions and execute each valid
command according to the rover's current position and direction.

FR-05 — Command Authentication
The system shall allow only authenticated Mission Control operators to issue commands.

FR-06 — Reject Invalid/Unauthorized Commands
The system shall reject commands that are invalid or unauthorized.

FR-07 — Command Execution Status
Mission Control shall receive the execution status of commands sent to the rover.

FR-08 — Event Logging
The system shall record all commands and critical rover events with a timestamp and operator ID.

FR-09 — Communication Failure Handling
The system shall continue operating despite temporary communication interruptions.

Non-Functional Requirements (NFRs)
Non-functional requirements describe how well or under what constraints the system must operate.

NFR-01 — Performance
Command processing should normally complete within 5 seconds after a command is received by the rover.

NFR-02 — Security
Only authenticated Mission Control operators shall be permitted to issue rover commands.

NFR-03 — Reliability/Availability
The system shall continue operating despite temporary communication interruptions.

NFR-04 — Scalability
The system should support communication with multiple rovers simultaneously.

NFR-05 — Communication Constraint
The system shall operate under limited communication bandwidth and several-minute communication delays.
