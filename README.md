# Lorenzzo Freitas Pagotti
**Gameplay Programmer — C++ & Unreal Engine 5**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lorenzzo-pagotti/)
[![Steam](https://img.shields.io/badge/Steam-Backrooms:_Collision_Not_Found-1b2838?style=flat-square&logo=steam&logoColor=white)](https://store.steampowered.com/app/4476610/Backrooms_Collision_Not_Found/)
[![Itch.io](https://img.shields.io/badge/Itch.io-The_Sleeping_Curse-FA5C5C?style=flat-square&logo=itchdotio&logoColor=white)](https://santodev.itch.io/thesleepingcurse)
[![Email](https://img.shields.io/badge/Email-lzpagotti%40gmail.com-333333?style=flat-square&logo=gmail&logoColor=white)](mailto:lzpagotti@gmail.com)

Gameplay Programmer specialized in **C++ and Unreal Engine 5**, focused on replicated multiplayer architecture, event-driven gameplay systems, and performance optimization. Solo developer of a commercial co-op title published on Steam and contributor to cross-disciplinary game production teams. Computer Science undergraduate (4th semester at PUC Goiás) currently open to **Gameplay / Unreal Engine Programming Internships and Junior roles**.

---

## Shipped & Commercial Projects

### [Backrooms: Collision Not Found](https://store.steampowered.com/app/4476610/Backrooms_Collision_Not_Found/) — *Solo Developer & Gameplay Programmer*
**Commercial Co-Op Title on Steam (Unreal Engine 5 | C++ & Blueprints)**
* **Commercial Release:** Architected, developed, and shipped a 1–4 player co-op horror/puzzle game as a solo developer, generating **$7,000+ in gross revenue within the first month**.
* **Multiplayer Architecture:** Engineered a Listen-Server network architecture with authoritative state management (`GameState`/`PlayerState`) and replication (`RPCs`, `RepNotify`) across Sanity, Stamina, Inventory, and synchronized multi-user puzzles.
* **Event-Driven Codebase:** Structured gameplay logic around Subsystems, Actor Components, and DataAssets, replacing unnecessary `Tick` polling with Delegates and Timers.
* **Optimization & Live Telemetry:** Profiled CPU/GPU bottlenecks via **Unreal Insights** (HISM, draw call reduction, PSO precompilation) to achieve **100+ FPS on integrated GPUs**, and integrated **Sentry** for post-launch crash triage.

### [The Sleeping Curse](https://santodev.itch.io/thesleepingcurse) — *Gameplay Programmer (Team of 15)*
**Scream Jam 2025 & Commercial Project (Unreal Engine 5 | C++ & Blueprints)**
* **Team Production:** Collaborated within a 15-person international team over a 10-month cycle on an Unreal Engine 5 title born in Scream Jam 2025 and expanded into a commercial release.
* **Core Gameplay & AI:** Architected a modular C++ character health/damage component, movement mechanics, monster AI behaviors, and interactive environmental puzzles, exposing clean Blueprint APIs (`UFUNCTION`/`UPROPERTY`) for level and game designers.

---

## Open-Source C++ Systems & Unreal Engine Plugins

Because the repositories for my commercial titles are private, the public repositories below showcase my C++ architecture, coding standards, and API design for Blueprint integration:

### 1. [UE-Gameplay-Systems-Library](https://github.com/LorenzzoPagotti/UE-Gameplay-Systems-Library)
A collection of modular, reusable C++ gameplay systems built for Unreal Engine 5:
* **AI System:** Custom C++ `AAIController` with `UAIPerceptionComponent` (sight and hearing configs), `BehaviorTree`, and custom C++ `UBTTaskNode` classes for patrol, investigation, pursuit, and search states.
* **Data-Driven Inventory:** Scalable inventory foundation built with `UDataAsset` and `USTRUCT` definitions for designer-friendly item authoring directly in the Unreal Editor.
* **Actor Attribute Components:** Event-driven Health and Stamina components communicating via C++ `UInterface` contracts and `Delegates`.

### 2. [UE-InteractionSystemPlugin](https://github.com/LorenzzoPagotti/UE-InteractionSystemPlugin)
A standalone **Unreal Engine C++ Plugin** providing a decoupled actor interaction framework:
* Built around C++ `UInterface` contracts to allow any actor to become interactable without hard class dependencies.
* Event-driven `Delegates` for zero-overhead UI prompt notifications and state updates.
* Fully exposed to Blueprints (`UFUNCTION`/`UPROPERTY`, `BlueprintCallable`, `BlueprintImplementableEvent`) for rapid designer workflow.

### 3. [UE-StaminaSprintPlugin](https://github.com/LorenzzoPagotti/UE-StaminaSprintPlugin)
A self-contained **Unreal Engine C++ Plugin** implementing a modular sprint and stamina management component:
* Stamina depletion, exhaustion handling, and regeneration logic.
* Plug-and-play `UActorComponent` architecture with full Blueprint API exposure for tuning movement speeds, stamina costs, and UI bindings in the editor.

---

## Technical Stack

* **Languages & Engine:** C++, Unreal Engine 5, Blueprints, Unreal Reflection System (`UPROPERTY`, `UFUNCTION`, `USTRUCT`, `UENUM`, `UInterface`)
* **Multiplayer & Gameplay Architecture:** Client-Server Replication, Listen-Server Authority, `RPCs` & `RepNotify`, `GameState`/`PlayerState`, Subsystems, Actor Components, DataAssets, Event-Driven Architecture (Delegates/Timers), AI (`BehaviorTree`, `AIPerception`)
* **Profiling, Telemetry & Tools:** Unreal Insights, HISM & Draw Call Optimization, PSO Caching, Sentry (Crash Triage), Git, GitHub, Visual Studio, JetBrains Rider
