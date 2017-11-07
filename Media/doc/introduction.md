# Media Data Models

These data models describe the main entities involved in multimedia sensor basing on computer vision. This pattern is based on using computer vision or speech analysis techniques to transform a device camera into an advanced sensor. Kurento provides, off-the-shelf, some basic computer vision capabilities for detecting faces, detecting crowds, detecting car plates, detecting movement, etc. Note that most of these analyses lead to generation of data that takes the form of events (e.g. detected a specific face, detected a car plate, detected an intruder, etc.)

You may want to manage these events as Context Information. These models represent the events that Kurento produces

The main entities identified are:

+ [MediaEvent](../MediaEvent/doc/spec.md). It represents a base for all events raised by elements in the Kurento media server
+ [PlateDetectedEvent](../PlateDetectedEvent/doc/spec.md). It represents an Event raised by a PlateDetectorFilter when a plate is found in the data streamed.
