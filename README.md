Phoenix AutoScribe

An Arduino-based automated handwriting machine capable of reproducing text using stepper motors and a servo-driven pen mechanism.

Components:
- Arduino UNO
- CNC Shield V3
- A4988 Drivers
- NEMA 17 Stepper Motors
- SG90 Servo Motor
- GT2 Belt System
- SMPS Power Supply

Features:
- Automatic writing
- CNC-based motion control
- Pen lift mechanism
- Custom text generation

Status:
Prototype under development.
+------------------+
                 |   Arduino UNO    |
                 +------------------+
                          |
                    CNC Shield V3
                          |
        ---------------------------------
        |               |               |
      X-Axis         Y-Axis         Servo
      A4988          A4988          SG90
        |               |             |
     NEMA17         NEMA17       Signal -> D11
   Stepper X      Stepper Y      VCC -> 5V
                                   GND -> GND

Power Supply (12V SMPS)
        |
        +------> CNC Shield V3
                     |
             Powers A4988 Drivers
             and Stepper Motors
