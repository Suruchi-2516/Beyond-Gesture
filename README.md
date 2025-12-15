 Interaction System (Air Canvas + Cursor)
Beyond Gesture is an experimental hand-gesture–driven interaction system that allows users to draw, create shapes, erase, and control a cursor in mid-air, using only a webcam — no mouse, no touchscreen.
The project explores natural human–computer interaction by blending gesture recognition, air-drawing, and touchless UI control into a single, real-time interface.

* Key Features
-Air Canvas
-Draw freely using pinch gestures
-Dynamic brush thickness based on finger distance
-Smooth stroke rendering with motion interpolation
-Shape Tool
-Draw rectangles, circles, and lines
-Live “ghost preview” before placing the shape
-Gesture-based scaling and placement
-Eraser Mode
-Touchless erasing using the same pinch gesture
-Adaptive thickness for precise control
-Touchless Cursor Mode
-Toggle between draw mode and cursor mode
-Move the cursor using your index finger
-Pinch gesture simulates mouse clicks
-Real-time Hand Tracking
-Single-hand tracking for lower latency
-Stable detection using MediaPipe Hands
-Minimal Hardware
-Works with a standard laptop webcam
-No external sensors or gloves required

*How It Works 
The webcam feed is captured in real time.
Hand landmarks are detected using MediaPipe Hands.
Key fingertip positions (index & thumb) are tracked.
Gestures are interpreted as:
-Pinch → Draw / Click
-Finger movement → Cursor / Brush motion
-Finger distance → Brush thickness & scaling
-Output is rendered on layered HTML5 canvases for smooth visuals.

* Gesture Map
Gesture	Action
-Index finger movement	Cursor / brush movement
-Index + thumb pinch	Draw / click
-Pinch + move	Continuous drawing
-Release pinch	Stop drawing / place shape
-Q key	Toggle cursor mode

 * Tech Stack
Frontend: HTML5, CSS3, JavaScript
Rendering: HTML5 Canvas (Base + Overlay)
Hand Tracking:
-TensorFlow.js
-MediaPipe Hands
-TensorFlow Hand Pose Detection
-Icons: Lucide Icons
-Runtime: Browser (WebGL enabled)

* Output Options

Clear Canvas – Reset the drawing area
Save PNG – Export your creation as an image

* Project Motivation
Traditional interfaces rely heavily on physical input devices.
Beyond Gesture explores an alternative interaction model where hand motion becomes the interface, opening possibilities for:
-Touchless systems
-Accessibility-focused interface
-Creative digital art tools
-Gesture-based UI experimentation
-This project is designed as a concept prototype, not a replacement for conventional input methods.

* Future Enhancements
 -Multi-hand support
 -Gesture-based mode switching (no keyboard)
 -Pressure-sensitive strokes
 -AI-assisted gesture customization
 -3D interaction space
