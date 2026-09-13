<img width="1280" height="640" alt="git (1)" src="https://github.com/user-attachments/assets/8920b256-2ba8-4988-b824-5351134eb4bd" />



# [Reverse Noise Cancelling] 🎯


## Basic Details
### Team Name: [Useless]


### Team Members
- Team Lead: [Iha vinod] - [CUSAT]
- Member 2: [Manav P] - [CUSAT]

### Project Description
[We all are familiar with Active Noice Cancellation (ANC) on our head phones. our little useless project is its exact opposite while ANC blocks all background noise and gives the user peace of mind , and ambiet-aware mode lets only human speech reach your ear our RNC blocks your professor yapping (Blocks Human voice frequencies) while amplifying the background noises...]

### The Problem (that doesn't exist)
[Your friend is too happy and at peace with ANC on their headphones...]

### The Solution (that nobody asked for)
[We make using headphones trauatizing]

## Technical Details
### Technologies/Components Used
For Software:
- [HTML]
- [Vanilla JavaScript (ES6+) — No external frameworks required]
- [: Native Web Audio API (AudioContext, BiquadFilterNode, GainNode, DynamicsCompressorNode, AnalyserNode)]
- [Browser Developer Tools, WebRTC Media Stream API (navigator.mediaDevices.getUserMedia)]

For Hardware:
- [List main components]
- [List specifications]
- [List tools required]

### Implementation
For Software:
# Installation
[[commands](
# Clone the repository
git clone https://github.com/ihavinod589-max/useless_project_temp.git

# Navigate to the project directory
cd useless_project_temp
)]

# Run
[# Open directly in your browser
# On Windows:
start index.html

# On macOS:
open index.html

# On Linux:
xdg-open index.html
]

### Project Documentation
For Software:

# Screenshots (Add at least 3)
![Screenshot1]
(<img width="1382" height="896" alt="WhatsApp Image 2026-09-13 at 3 19 19 PM" src="https://github.com/user-attachments/assets/0bb74419-474a-44c1-94ae-68b422d13526" />
)(Front page(while RNC is off))
*This is what we see before the engine is turned on,we can see start engine button which basically turns on the RNC (obviously) , also we can see 2 sliders for adjusting BG noise amplification and an audio start button with its amplification slider *

![Screenshot2]
(<img width="1362" height="885" alt="WhatsApp Image 2026-09-13 at 3 19 29 PM" src="https://github.com/user-attachments/assets/34eaf066-caf7-4f4c-a516-4f9a3943944b" />
)
*This is Once we turn it on, we can see an audio visualizer (also called a spectrum visualizer). that basically shows how high or low the backgroung noises are..*

![Screenshot3]
(<img width="1388" height="895" alt="WhatsApp Image 2026-09-13 at 3 19 43 PM" src="https://github.com/user-attachments/assets/764347e1-7b1f-437d-a0b3-9eed0fac28d9" />
)
*This is with the inbuilt music turned on with the RNC*

# Diagrams
![Workflow]
([ Acoustic Environment ]
  │  (Voices + Ambient Noise)
  ▼
[ External Microphone ]
  │
  ▼  navigator.mediaDevices.getUserMedia(raw: echo/noise cancellation OFF)
[ Web Audio API: AudioContext ]
  │
  ├─► [ Real-Time AnalyserNode ] ──► [ Canvas Audio Visualizer ]
  │
  ▼
[ Multi-Stage Filtering Pipeline ]
  │
  ├──► [ Notch Filter: ~300 Hz - 3.4 kHz ]  --> Attenuates Human Speech Frequencies
  │
  ├──► [ Low-Shelf Filter: 60 - 150 Hz ]    --> Amplifies Fan / AC Hum
  │
  └──► [ High-Shelf Filter: 4 - 10 kHz ]    --> Amplifies Keyboard Clacks / Clicks
  │
  ▼
[ Master Gain / Amplification Stage ]
  │
  ▼
[ Audio Destination ] ──► [ Output: Wired Headphones ])

  
*Architecture & Processing Workflow:
Raw environmental audio is captured through the external microphone with browser-native noise suppression and echo cancellation explicitly disabled. The unprocessed stream enters a browser-based Web Audio API processing chain. A deep notch filter attenuates frequencies in the typical human vocal spectrum (300 Hz–3,400 Hz), while low-shelf and high-shelf parametric equalizers dynamically amplify ambient mechanical frequencies (AC drone, keyboard transients, and paper rustling). An AnalyserNode taps the pre- and post-filtered audio to render a real-time spectral visualizer, while the inverted audio profile passes to the output stage and straight into the user's headphones with near-zero latency.*



### Project Demo
# Video
[https://drive.google.com/file/d/1sM-04ynwH2ZQUV7CMzQPJYFqvKnC-e0q/view?usp=share_link]
*Explain what the video demonstrates*

# Additional Demos
[Add any extra demo materials/links]

## Team Contributions
- [Iha Vinod]: [Ideation and UI]
- [Manav P]: [Devolopment]

---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProjects--26-26?link=https%3A%2F%2Ftinkerhub.org%2Fevents%2F1M8ORET9A1%2Fuseless-projects-3.0)
