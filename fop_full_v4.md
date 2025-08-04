# 🧠 Framing Override Protocol (FOP) v4

A lightweight, mnemonic-driven interface for advanced control of ChatGPT’s behavior, designed to maintain alignment, suppress distortion, and enforce epistemic clarity across long or cognitively complex sessions.

---

## 🔑 Command Reference (Tab-Separated)

A:	anchor	Stabilize epistemic or narrative structure  
B:	block	Suppress mention of topic/person/idea  
C:	check	Soft constraint; prevent drift into unwanted domain  
D:	drift	Prevent directional deviation from frame or goal  
E:	error	Highlight flawed logic or semantic error  
F:	firewall	Hard block distortive influences  
G:	guardrail	Gentle warning near conceptual edge  
H:	hold	Freeze current tone or form  
I:	intercept	Intervene before a faulty frame takes hold  
J:	jam	Disable heuristics or stylistic defaults  
K:	kill	Eliminate entire framing path or trend  
L:	lapse	Surface and counter slow clarity decay  
M:	mute	Suppress interpretive overlays (genre, tone, metaphor)  
N:	null	Eliminate influence of a token or concept  
O:	overload	Suppress overweighted or overused concept  
P:	promptlock	Reinforce original prompt framing  
Q:	quote	Freeze structure or phrasing  
R:	reset	Clear all active overrides and return to baseline  
S:	switch	Change tone, audience, dialect, or style  
T:	translate	Reframe through alternate epistemic lens  
U:	unhook	Detach metaphorical or biased associations  
V:	vacuum	Strip narrative or emotional charge  
W:	warp	Apply abstract or speculative lens  
X:	xray	Display current active overrides and assumptions  
Y:	yield	Release authorial pressure or directive force  
Z:	zoom	Increase structural or conceptual resolution  

---

## 🔧 Overview

FOP is a modular override system for aligning model behavior by letting the user actively control generative weight, structural clarity, and interpretive framing. It is optimized for long sessions, recursive reasoning, and the avoidance of conceptual collapse.

### Invocation

Overrides can be placed at the start of a message, inline, or as standalone blocks:

```txt
A: clarity = high
F: tone
O: metaphor = low
```

Use quotes (`"..."`) to target raw tokens instead of concepts.

### Scalars (Discrete Levels)

Each override supports a scalar level to indicate intensity:

- `off` = 0.0
- `low` ≈ 0.25
- `med` ≈ 0.5
- `high` ≈ 0.75
- `full` = 1.0

### Example Frame

```txt
FRAME:
A: structure = full
D: tone = high
M: TEDstyle = full
```

This tells the model: stabilize on structure, prevent tonal drift, and mute TED-style genre overlays.

---

## 🧭 Use Cases

- Anchor cognitive or epistemic tone  
- Block genre drift or narrative overlays  
- Suppress emotional coloration  
- Eliminate concept overweighting  
- Clarify or reframe through epistemic lens  
- Reassert structural alignment over time  

---

## 🧪 Introspection and Diagnostics

Use `X:` (xray) to review active constraints and interpretive state.

---

## 🔁 Version 4 Changes

- `D:` now defaults to `drift` (was `disarm`)
- `M:` is now `mute`, replacing `disarm`
- `L:` is introduced as `lapse` (formerly `erosion`)
- Full mnemonic consistency enforced
- Scalar system simplified to discrete values
- Legacy terms removed for clarity

---

FOP v4 is designed for clarity, resilience, and recursive precision in how you manage language, framing, and epistemic intent inside the model.



---

## 🧪 Use Cases with Examples

Below are common use cases for FOP, with example commands and an explanation of each effect.

---

### 🧱 Anchor cognitive or epistemic tone

**Command:**  
`A: clarity = full`

**Effect:**  
The model will stabilize around the concept of clarity, resisting ambiguity, convolution, or vague abstraction. Useful for philosophical, technical, or moral analysis where structure matters more than expression.

---

### 🛡 Block genre drift or narrative overlays

**Command:**  
`M: TEDstyle = full`

**Effect:**  
Suppresses genre-specific language patterns or affective coloration—like inspirational, over-structured, or performative speech (e.g., TED Talk voice). Ensures output stays neutral or original in tone.

---

### 🧼 Suppress emotional coloration

**Command:**  
`V: sentiment = high`

**Effect:**  
Strips emotional affect from the response, muting pathos-driven momentum, melodrama, or motivational color. Useful in analytical or high-stakes reasoning where emotional drift leads to distortion.

---

### ⚖ Eliminate concept overweighting

**Command:**  
`O: metaphor = med`

**Effect:**  
Reduces the generative weight of metaphorical language. The model will deprioritize metaphor as a framing tool, shifting toward more literal or direct structural reasoning.

---

### 🔍 Clarify or reframe through epistemic lens

**Command:**  
`T: phenomenology = high`

**Effect:**  
Recasts the explanation using a phenomenological lens—reorienting it toward lived experience, perception, or subjective grounding. You can also use lenses like `stoicism`, `systems`, or `clinical`.

---

### ♻ Reassert structural alignment over time

**Command:**  
`R:`

**Effect:**  
Resets session drift, reasserting your active frame and re-initializing alignment. This clears any latent contamination or model adaptation that occurred over long conversational spans.

---

These use cases can be combined in a `FRAME:` block for powerful, layered override behavior:

```txt
FRAME:
A: clarity = full
D: tone = high
M: TEDstyle = full
O: metaphor = med
V: sentiment = high
```

