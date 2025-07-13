
# 🧠 FractiAgent™

**The Layered Intelligence Engine for Purpose-Aligned Agents**  
Powered by FractiData • Runs in Docker • Built for LangChain / Pinecone / Python apps

---

## 🌍 Overview

**FractiAgent™** is a universal prompt + agent engine that detects the user's active **Fractal Intelligence Layer (0–7)**, identifies their **archetypal story pattern**, and returns the **least-cost, highest-benefit next action** using PEFF (Paradise Energy Fractal Force) logic.

This repo includes:

- 🔌 API-ready prompt logic
- ⚙️ Python class module (plug into LangChain, CrewAI, OpenAI Assistants, etc.)
- 🐳 Docker container setup
- 🧠 Integration with FractiData (Pinecone + LangChain genetic chains)
- 🧪 Real-world test cases
- 🔁 UI-ready API response format

---

## 📦 Architecture

```text
[Docker Container]
├── FractiAgent (Core logic + prompt)
├── LangChain (prompt orchestration)
├── Pinecone (memory, vector DB)
├── FractiData API (calls to store/retrieve/use fractalized insights)
└── Apps → UI / API / Assistants / Tools


⸻

🚀 Quick Start

1. Clone the Repo

git clone https://github.com/fractiverse/fractiagent.git
cd fractiagent

2. Launch Docker Container

docker build -t fractiagent .
docker run -p 8080:8080 fractiagent

3. Call the Agent

Send a request to localhost:8080/evaluate:

{
  "text": "I'm stuck in a power struggle with my co-founder."
}

Response:

{
  "active_layer": 3,
  "story_pattern": "Hero vs Shadow",
  "recommended_move": "Upgrade to Layer 4: Logic/Structure—facilitate shared decision framework.",
  "expected_benefit": "Dissolves power tension; aligns vision; restores trust."
}


⸻

🧠 Fractal Intelligence Layer Model

Layer	Name	Theme
0	Infinite	All possibilities
1	Instinct	Survival / Fear
2	Tribe	Emotion / Belonging
3	Power	Conflict / Drive
4	Logic	Systems / Process
5	Fractal Awareness	Meta / Pattern view
6	Purpose Alignment	Mission / Legacy
7	Harmony	Unity / Flow


⸻

🧰 FractiAgent Logic

class FractiAgent:
    def detect_layer(self, text): ...
    def archetype(self, text): ...
    def recommend(self, layer): ...
    def evaluate(self, text): ...

See agent.py for full source.

⸻

🔁 API Endpoint

POST /evaluate

Request:

{
  "text": "My team is overwhelmed and lacking clarity."
}

Response:

{
  "active_layer": 2,
  "story_pattern": "Tribal Overload",
  "recommended_move": "Upgrade to Layer 4: Introduce shared OKRs and roadmap clarity.",
  "expected_benefit": "Restores alignment; reduces burnout; improves output quality."
}


⸻

🔗 FractiData Integration

FractiAgent calls into FractiData modules to access:
	•	🔍 Genetic chain insights (LangChain + Pinecone)
	•	🧠 Context memory for long-term goals
	•	🔢 Tokenized thought-structure from past sessions

Set your FRACTIDATA_API_KEY and connect in config.py.

⸻

💡 Use Cases

Domain	Challenge	Benefit via FractiAgent
Product Strategy	Too many features, unclear vision	Detects L4 → Elevates to L6 purpose fit
Team Conflict	Ego battles, emotional tension	Detects L2/3 → Frames L4 or L5 structure
Personal Burnout	“I’m exhausted, can’t see the why”	Detects L6 → Recommends L7 + recovery pattern
Writing Block	Blank page fear	Detects L3 → Reframes L5 fractal plot outline


⸻

📱 Integrate with Any App

# Python Client Example
from fractiagent import FractiAgent

agent = FractiAgent()
response = agent.evaluate("I feel stuck in old habits and can’t move forward.")

print(response)

{
  "active_layer": 3,
  "story_pattern": "Hero vs Shadow",
  "recommended_move": "Layer-up to 5: Recognize repeating pattern, break cycle.",
  "expected_benefit": "Initiates breakthrough; reclaims agency."
}


⸻

🔧 Developer Notes
	•	Python ≥ 3.9
	•	Requires LangChain, Pinecone client, FastAPI (optional)
	•	Dockerfile included
	•	FractiData connection via config.py

⸻

🧬 License & Credits

© FractiVerse Labs 2025 • Open-source for non-commercial use.
Built with love using FractiScope, PEFF, and fractal cognition frameworks.
FractiAgent™ is part of the larger FractiVerse.