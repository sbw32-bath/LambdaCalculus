# 🧩 Functionia: The Lambda Loom

> *“Apply... define... become...”*

Welcome to **Functionia: The Lambda Loom**, a symbolic, narrative-driven puzzle game that weaves abstract thought, logic, and identity through a beautifully stylized Unreal Engine world grounded in the principles of **lambda calculus**.

---

## 🌌 Story Overview

Functionia was once a radiant realm, where reality itself was shaped by pure thought through the metaphysical **Lambda Loom**. But after the catastrophic **Reduction Collapse**, logic, time, and meaning fractured. You are the **Syntax Seeker**, drawn from the rigid realm of *Imperativa*, guided only by the ancient symbol: `λ`.

Your journey: to reawaken the Lambda Loom and restore **foundational principles**—identity, abstraction, recursion, truth, logic gates, and more.

---

## 🛠️ Development Overview

- **Engine**: Unreal Engine 5+
- **Project Template**: Third/First Person
- **Core Systems**:
  - Enhanced Input System
  - Custom Game Mode & Player Controller
  - Modular Blueprint architecture

---

## 🗺️ Chapter 1: Awakening Thought (Blank Village)

### 🔲 Environment: The Monochromatic Canvas

- **Visual Design**: Minimalist, wireframe-like ruins of logic
- **Progression Mechanic**: Objects and environment "bloom" into color as logical principles are applied

### 🧱 Key Assets

- Inert Buildings (basic shapes)
- Faded Scrolls (hidden knowledge)
- Broken Tools (e.g., torch, pump)
- **The Lambda Stone** (first awakening)

### 🎨 Materials & Effects

- **Color Bloom Shader**:
  - Master Material with grayscale-to-color Lerp
  - Dynamic Material Instances updated via Blueprint Timelines
- **Emissive Glow**: Awakening feedback
- **Post-Processing**:
  - Global desaturation on start
  - Gradual color restoration as puzzles are solved

---

## 🧍‍♂️ The Player: Syntax Seeker

- Stylized character model (ethereal/silhouette)
- Standard movement
- Proximity-based interaction system (collision + prompts)

---

## 🧠 Core Gameplay: The Lambda Loom System

### 🎛️ UI & Expression Building (UMG)

- Drag-and-drop interface with:
  - `λ`, variables (`x`), values (`water`, `sun_dial`, etc.)
  - Visual representation of lambda expressions
- Expression evaluation button
- Conditional glyph unlocking via global Game State

### 🧩 Evaluation Mechanics

- **Beta Reduction Logic**: `(λx. x) water → water`
- **Expression Parsing**: Handled via Player Controller or `BP_LambdaEvaluator`

### 🧿 Visual Feedback

- Glyph animations during evaluation
- Object awakening: color, particles, sounds, and glow

---

## 🔓 Puzzles & Progression

### 📍 Stage 1 Tasks

- **Awakening the Lambda Stone**:
  - Unlocks `λ` and variable glyphs
- **Identity Function Puzzle**: `(λx. x) value`
  - Activate Fountains & Sun Dials
- **Scroll Decoding**: `(λx. x) scroll_content`
  - Reveals written knowledge of identity and reduction
- **Sign Restoration**: Combine glyphs to restore meaning

### 🌐 Game State Management

- `UnlockedGlyphs[]`, `AwakenedObjects[]` stored in GameInstance
- Conditional visibility for puzzles and UI

---

## 🔊 Visual & Audio Design

- **Soundscape**:
  - Initial silence, building ambient track
  - Object-specific cues (fountain gurgles, chimes, pulses)
- **Glow Effects**:
  - Niagara-based particles for reactivated objects
- **Scroll Animation**:
  - Revealing glyphs using wipe/dissolve effects

---

## ⚙️ Best Practices (UE5)

- Blueprint-first development
- Use Data Assets for puzzle content
- Create a parent `BP_AwakeningObject` for scalable design
- Optimize materials and particles for performance
- Leverage Unreal’s debugging tools extensively

---

## 📚 Educational Theme

Functionia introduces players to core **lambda calculus** concepts in an intuitive, experiential way:
- Identity functions
- Abstraction
- Beta reduction
- Evaluation of expressions
- Recursive problem-solving

---

## 📁 Folder Structure Suggestion

```plaintext
/Functionia
│
├── /Blueprints
│   ├── Characters/
│   ├── Glyphs/
│   ├── Interactables/
│   └── UI/
│
├── /Materials
├── /Niagara
├── /Sounds
├── /UI
└── /DataAssets
