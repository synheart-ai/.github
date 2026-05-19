<!-- Centered hero section -->
<div align="center">

<img src="../assets/SynHeart_logo_brand_Gradient.png" alt="Synheart Logo" width="780"/>

Beep Boop.

**Make Computers Feel Human**  

[![Website](https://img.shields.io/badge/Website-synheart.ai-0ea5e9?style=flat-square)](https://synheart.ai)
[![License](https://img.shields.io/badge/license-Apache--2.0-blue?style=flat-square)](#license)
[![Source Available](https://img.shields.io/badge/source-available-22c55e?style=flat-square)](#contributing)

</div>

---

## 🌍 What is Synheart?

**Synheart** is an open, privacy-preserving **Human State Interface (HSI) infrastructure** that enables software systems to understand human emotional, cognitive, and behavioral state — without relying on explicit user input.

Instead of clicks, prompts, or surveys, Synheart derives **human state from multimodal signals** — physiological, behavioral, and contextual — processed locally and represented in a standardized format.

At the core of Synheart is **HSI** — a **canonical, language-agnostic JSON contract** for representing human state across independent systems.

> HSI plays a role similar to GPS or HTTP — a shared communication standard for human state.

---

## 🧠 The Synheart Stack

Synheart is organized as composable layers. Each layer emits or consumes well-defined contracts — adopt only what you need.

### 📡 Signal Layer
Vendor- and platform-agnostic capture of multimodal signals.
- **Synheart Wear** — biosignals from wearables (Apple Watch, Pixel Watch, Garmin, …)
- **Synheart Sensor Agent** — host-device and ambient sensor capture
- **Synheart Edge** — on-device kernels for low-level signal processing

### ⚙️ Runtime
The load-bearing piece — turns raw signals into derived features and real-time scores that the Interpretation Layer rides on.
- **Synheart Engine** — high-performance signal processing pipeline. Closed-source binary, distributed via the Synheart CLI:
  ```bash
  curl -fsSL https://synheart.sh/install | sh   # install the CLI
  synheart install runtime                      # install the engine
  ```

### 🧩 Interpretation Layer
Modules that turn signals into human state. All emit **HSI-compliant** outputs.
- **Synheart Emotion** — emotional dynamics (stress, calm, arousal, valence) from physiological signals
- **Synheart Focus** — cognitive engagement, attention stability, and mental load over time
- **Synheart Behavior** — behavioral patterns from interaction and usage dynamics

### 🪟 Session Layer
- **Synheart Session** — windowed human state with context, scoring, and continuity across activities

Every layer is **composable, interoperable, and optional** — systems can adopt only what they need.

---

## 🧩 Architecture Overview

```text
[ Wearables • Host Sensors • Ambient ]
Apple Watch • Pixel Watch • Phone • Desktop • …
↓
Signal Layer
Synheart Wear • Sensor Agent • Edge
↓
Runtime
Synheart Engine
↓
Interpretation Layer
Synheart Emotion • Focus • Behavior
↓
Session Layer
Synheart Session
↓
HSI (canonical human-state JSON)
↓
Your System (AI • Interfaces • Agents • Apps)
```


## ⚙️ Cross-cutting Components

| Component | Description |
| --- | --- |
| 🧠 **HSI** | The authoritative human-state interface specification |
| 📦 **SDKs** | Platform SDKs (Rust, Flutter, Kotlin, Swift) for on-device integration |
| 📄 **Whitepapers** | Open research and technical documentation |

---

## 🔐 Privacy by Design

- **On-device processing by default**
- **No raw signals required to leave the device**
- **Derived state only (HSI outputs)**
- **Consent-gated cloud sync (optional)**

Synheart is built to support **ethical, human-centered computing** from the ground up.

## 🚀 Tech stacks

### These are us and our AI agents play around :) 

- Rust (engine & core runtime)
- Flutter
- Kotlin
- Swift
- Go
- Python
- TS

More SDK-specific setup is available in each package’s README and in `docs/`.


---



## 💡 Why Synheart?

- 🧠 Standardized human state — not ad-hoc emotion labels
- 🔐 Privacy-preserving by default
- 🧩 Modular and extensible
- 🌍 Vendor- and platform-agnostic
- 📄 Open source with open research

Synheart is not an app, model, or agent.

It is infrastructure for human-state-aware systems.

---

## 🗺️ Roadmap

- Evolving HSI schema
- Additional state interpreters
- On-device kernels
- Reference integrations
- Research benchmarks

---

## 🤝 Contributing

Synheart is **source-available** — the code is published for you to read, audit, and learn from, but development happens in-house.

- ✅ **Issues welcome** — bug reports, questions, and feature requests via GitHub Issues on the relevant repository
- ❌ **Pull requests are not accepted** at this time

See `REPOSITORY_IMPLEMENTATION_GUIDELINES.md` for repo conventions.

---

## 🔒 License

Licensed under the Apache 2.0 License.
© 2025–2026 Synheart AI.

---

<div align="center">

🫶 "Human state is a first-class signal."

🌐 [synheart.ai](https://synheart.ai) • [LinkedIn](https://www.linkedin.com/company/synheart/) • [X](https://x.com/synheart_ai)

</div>