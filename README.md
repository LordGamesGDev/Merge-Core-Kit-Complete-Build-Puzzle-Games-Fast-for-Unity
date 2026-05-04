# 🧩 Merge Core Kit – Build Puzzle Games Fast
**Production-ready • Scalable Architecture • Cross-Platform Support**

Merge Core Kit is a fully functional, extensible 2D merge game template built for Unity. Inspired by the popular physics-based merge genre, it provides a clean, modular foundation for building commercial-quality games without rewriting core systems.

This is not a prototype. It is a structured, maintainable framework designed for real production use.

---

## 🪄 Key Features

- Complete gameplay loop: spawn → physics → merge detection → scoring → game over
- Interface-driven architecture (`IGameService`, `IMergeable`, `IInputProvider`, `IScoreCalculator`)
- Generic object pooling system to eliminate runtime allocations and GC spikes
- ScriptableObject-based data pipeline for content-driven design
- Cross-platform input system (Mouse, Touch, Keyboard)
- DOTween-powered UI animations
- Audio system with pitch scaling based on merge level
- Persistent scoring and settings via PlayerPrefs
- Designed for PC, macOS, iOS, Android, and WebGL

**Requirements:**
- Unity 2022.3 LTS or newer
- DOTween
- TextMeshPro

---

## 🎸 Architecture Overview

The template is structured into independent systems with clear separation of concerns:

- **GameManager** – Application entry point and system orchestration
- **GameSession** – State machine and game flow control
- **MergeSystem** – Core merge validation and resolution logic
- **ObjectPooler** – Memory-safe object lifecycle management
- **ScoreService** – Scoring and persistence layer
- **AudioManager** – Music, SFX, and UI audio with per-channel volume control
- **SpawnController** – Controlled spawn and input handling

All cross-system communication is handled through C# events.
Gameplay logic is fully decoupled from the UI layer, allowing complete UI replacement without modifying core gameplay code.

---

## 🎨 Fully Customizable

The system is content-driven and theme-agnostic. You can:

- Replace fruit assets with any theme (bubbles, planets, icons, etc.)
- Modify scoring logic via custom `IScoreCalculator` implementations
- Add new game modes by extending or composing `GameSession`
- Adjust merge chains through `MergeTable` configuration

Core systems do not require modification for common customizations.

---

## 📖 Included Documentation

- Detailed system breakdown
- Architecture explanation
- Interface reference
- Setup and Quick Start guide
- Customization instructions
- Troubleshooting section
- License and commercial usage terms

Music by Arseniy Popov is included and cleared for commercial use within finished products.

---

Fruit Merge Kit provides a structured foundation for developers who value clean architecture, extensibility, and production stability.
