<div align="center">

# Yuri Ornellas 👋

### Junior Game Development · Technical Game QA · Technical Operations

**Unity 6 · C# · NUnit · Unreal Engine 5 · Blueprints · Python · GitHub Actions · Linux**

📍 Brazil · Open to international remote opportunities and relocation

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yurivillarornelas/)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:yurivillarornelas@live.com)
[![GitHub](https://img.shields.io/badge/GitHub-Projects-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ornellasdev)

</div>

---

## About me

I'm a Brazilian IT and esports professional moving into game development and technical game QA. I build small playable prototypes so I can follow a problem from the player's input through gameplay code, collision and on-screen feedback. My background includes systems support, incident investigation and technical operations.

## Portfolio highlights

| Engine | What I built and tested | Start here |
| --- | --- | --- |
| **Unity 6.6** | A C# sandbox for health, damage, checkpoints and respawn. I test model boundaries in Edit Mode and scene behavior in Play Mode. | [29 local Unity tests with screenshots and execution records](https://github.com/ornellasdev/unity-qa-sandbox/blob/main/Docs/TEST_EXECUTION_REPORT_RUN-008.md) |
| **Unreal Engine 5.9 Preview 2** | A Blueprint control room with two terminals and a powered security door. I investigate what players can see, when their inputs take effect and whether they can pass the moving door. | [How I found and fixed a readability issue in the control room](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab#case-study--making-the-control-room-terminals-readable) |

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ornellasdev&amp;layout=compact&amp;theme=dracula&amp;title_color=58A6FF" alt="Most used languages in Yuri's public repositories" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=ornellasdev&amp;show_icons=true&amp;theme=dracula&amp;custom_title=Yuri%20Ornellas%27%20GitHub%20Stats&amp;title_color=58A6FF&amp;ring_color=58A6FF" alt="Yuri Ornellas' GitHub activity statistics" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Unity-Dark.svg" width="42" height="42" alt="Unity" title="Unity" />
  <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/CS.svg" width="42" height="42" alt="C#" title="C#" />
  <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/UnrealEngine.svg" width="42" height="42" alt="Unreal Engine" title="Unreal Engine" />
  <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Python-Dark.svg" width="42" height="42" alt="Python" title="Python" />
  <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/GithubActions-Dark.svg" width="42" height="42" alt="GitHub Actions" title="GitHub Actions" />
  <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Linux-Dark.svg" width="42" height="42" alt="Linux" title="Linux" />
</p>

## Unity QA Sandbox

The player can move, jump, take damage, activate a checkpoint and respawn. One question guided my testing: when health reaches zero after a checkpoint, do the health model, respawn position and scene triggers agree? [Project and playable scene](https://github.com/ornellasdev/unity-qa-sandbox#run-the-project-and-tests-locally)

| Layer | Evidence |
| --- | --- |
| **C# and NUnit · local Unity Editor** | **22/22 Edit Mode** tests passed for health and checkpoint models, including invalid inputs and large healing values. **7/7 Play Mode** tests passed for damage, health recovery, physical triggers and scene integration. RUN-008 includes Test Runner screenshots and before/after Git snapshots, which recorded local changes during execution. [Unity RUN-008](https://github.com/ornellasdev/unity-qa-sandbox/blob/main/Docs/TEST_EXECUTION_REPORT_RUN-008.md) |
| **Regression investigation** | An earlier full-scene run passed 4 of 7 Play Mode tests. After adjusting scene loading and teardown, the retest passed all 7. [Investigation and retest](https://github.com/ornellasdev/unity-qa-sandbox/blob/main/Docs/TEST_EXECUTION_REPORT_RUN-006.md) |
| **Manual gameplay QA** | Four cases covered movement, jumping, collision and respawn. The clip shows damage and health recovery. [Manual report](https://github.com/ornellasdev/unity-qa-sandbox/blob/main/Docs/TEST_EXECUTION_REPORT_RUN-002.md) · [Gameplay clip](https://github.com/ornellasdev/unity-qa-sandbox/blob/main/Evidence/RUN-002-Gameplay-Respawn.mp4) |
| **GitHub Actions · static checks** | CI validates repository structure and scans C# syntax and Unity-specific patterns. The recorded run checked 13 C# files with zero findings. The Python analyzer passed **35/35** regression tests with **98.1% line coverage** of its own code. Hosted Unity Test Runner execution remains a roadmap item. [Verified CI run](https://github.com/ornellasdev/unity-qa-sandbox/actions/runs/45102487210) |

**Try it:** open the project in Unity Hub with editor `6000.6.10f1`, load `Assets/Scenes/QASandbox.unity` and press Play. To repeat the local suites, open **Window → General → Test Runner** and run Edit Mode and Play Mode separately. [Setup and test commands](https://github.com/ornellasdev/unity-qa-sandbox#run-the-project-and-tests-locally)

## Unreal Engine 5 Technical QA Lab

**[How I found and fixed a readability issue in the control room](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab#case-study--making-the-control-room-terminals-readable).** Four gameplay tests passed, yet the recording showed a player-facing defect. Pressing E restored power, but the terminal gave no readable confirmation. I moved the label onto the terminal face, adjusted the lighting and connected the display to the Blueprint state. At the same interaction point, the player can now read **POWER ON**.

| Before the fix | After the fix |
| --- | --- |
| ![Power terminal face with no readable confirmation](https://raw.githubusercontent.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/9d9e5e061f75c4b3f65e894c71a026e7f33b4ebe/qa/case-studies/terminal-readability/before.jpg) | ![Power terminal labeled POWER with POWER ON visible after interaction](https://raw.githubusercontent.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/9d9e5e061f75c4b3f65e894c71a026e7f33b4ebe/qa/case-studies/terminal-readability/after.jpg) |

| Layer | Evidence |
| --- | --- |
| **Gameplay regression · local Unreal sessions** | **6/6** cases passed on Linux. They cover an unpowered door, interaction range, repeated input and collision during opening. One probe moved the player just **2 cm** across the terminal's interaction boundary. [Range boundary](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/blob/main/qa/runs/RUN-005/README.md) · [Six-case results](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/blob/main/qa/runs/RUN-006/README.md) |
| **Collision investigation** | With forward input held, I sampled the player and door positions at **30, 60 and 120 simulated fps**. The player cleared the panel 0.617–0.633 simulated seconds after opening began. [Measurements and reproduction steps](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/blob/main/qa/runs/RUN-007/README.md) |
| **Native Blueprint test · Unreal Automation** | A Functional Test Actor presses E, reads the terminal's Text Render component and checks that the unpowered door stays closed. The editor reported **1 pass, zero warnings and zero errors**. [Blueprint and exported result](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/blob/main/qa/runs/RUN-008/README.md) |
| **Exploratory and visual QA** | I checked the new messages from the player's viewpoint, then probed re-entry during motion, repeated inputs after opening and reset in a fresh session. [Visual retest](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/blob/main/qa/runs/RUN-002/README.md) · [Exploratory report](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/blob/main/qa/runs/RUN-003/README.md) |
| **GitHub Actions · log verification** | Five Python tests replay recorded evidence. They check that the verifier accepts valid runs and rejects a duplicate opening, a missing sample or passage through a closed door. [Verified CI run](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/actions/runs/45730585349) |

**Try it:** open `ControlRoomLab.uproject` in Unreal Engine 5.9 Preview 2. Move with WASD, look with the mouse and press E at each terminal. To inspect the native test, search for **UnpoweredDoor** in **Session Frontend → Automation**. [Gameplay clip](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab/blob/main/qa/runs/RUN-001/control-room.mp4) · [Local regression command](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab#run-the-functional-regression)

## Skills and toolkit

- **Gameplay programming:** C# components and models in Unity, Blueprint interactions and state transitions in Unreal.
- **Technical QA:** exploratory charters, negative and boundary cases, collision sampling, defect reproduction, visual retesting and execution reports.
- **Automation and tooling:** NUnit, Unity Test Framework, Unreal Functional Testing, Python, Tree-sitter C#, GitHub Actions and Bash on Linux.
- **Technical operations:** incident investigation, troubleshooting, documentation and cross-team coordination.

## Portfolio roadmap

- **Unity:** extend video evidence for the initial and checkpoint respawn paths and evaluate licensed CI for the Unity test suites. [Unity roadmap](https://github.com/ornellasdev/unity-qa-sandbox#roadmap)
- **Unreal:** the next proposed milestone is an acceptance test of a packaged Linux build, covering startup, controls, terminal feedback, passage and restart. [Completed Unreal runs](https://github.com/ornellasdev/Unreal-Engine-5-Technical-QA-Lab#test-runs-and-evidence)

## Esports experience

I bring **12+ years of esports involvement**, including competitive operations, coaching, team management and tournament-related projects, with experience associated with **ESL Gaming, INTZ and Isurus Gaming**.

Competitive esports strengthened my communication, high-pressure troubleshooting, collaborative decision-making and understanding of player experience — skills I am now applying to game development and QA.

## Education and certifications

- Bachelor's Degree — Computer Engineering
- Bachelor's Degree — Advertising & Social Communication
- MBA — Project Management & Agile Methodologies
- ISO/IEC 27001 Lead Auditor
- ITIL Foundation
- Scrum Master Professional Certification

## Open to opportunities

I'm interested in **Junior Game QA / QA Tester, Technical QA, Junior Game Developer, and Game Development Support** roles, especially with international studios.

**Languages:** Portuguese (native) · English (fluent) · Spanish (intermediate)  
**Location:** Brazil · Open to remote work and relocation

---

<div align="center">

### Let's build and test better games.

[LinkedIn](https://www.linkedin.com/in/yurivillarornelas/) · [Email](mailto:yurivillarornelas@live.com) · [GitHub](https://github.com/ornellasdev)

<sub>Portfolio work shown here is self-directed learning and project experience, not a claim of prior paid studio Game QA employment.</sub>

</div>
