## System Block Diagram (Input → Process → Output)

```mermaid
flowchart TD
    I["Input
    Hand Gestures
    (Webcam)"]

    P1["Process
    Gesture Recognition System
    (MediaPipe + OpenCV)"]

    P2["Process
    Car Movement Commands
    (Protocol Mapping)"]

    P3["Process
    Communication Bridge
    (Host → Car via Serial)"]

    P4["Process
    Arduino Board
    (Master / Slave Control)"]

    O["Output
    Car Motor Control Unit
    (Vehicle Movement)"]

    I --> P1
    P1 --> P2
    P2 --> P3
    P3 --> P4
    P4 --> O
