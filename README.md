flowchart TD
    I["Input
    Hand Gestures via Webcam"]
    
    P1["Process
    Gesture Recognition System
    (MediaPipe + OpenCV)"]
    
    P2["Process
    Command Mapping
    (Movement Protocol)"]
    
    P3["Process
    Communication Bridge
    (Python → Serial)"]
    
    P4["Process
    Arduino Controller
    (Master/Slave Logic)"]
    
    O["Output
    Car Movement
    (Forward / Backward / Left / Right / Stop)"]

    I --> P1
    P1 --> P2
    P2 --> P3
    P3 --> P4
    P4 --> O
