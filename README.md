# 🧭 Grid Coverage Planning AI (Showcase)

Classical AI · Graph Search · DFS Traversal · Plan Verification · Plan Synthesis

This repository is a **public showcase** of my Classical AI project on **grid coverage planning** in a toroidal grid-world.
✅ Documentation is public  
🔒 Implementation code is private (available upon request for academic/professional review)

---

## 🔒 Code Access
The full implementation is maintained in a **private repository** to prevent unrestricted reuse.
If you are a recruiter, researcher, or instructor and would like to review the code, please contact me.

---

## 📌 Problem Summary
The environment is a **2D grid cave** containing:
- Free tiles (must be visited/cleaned)
- Walls (`X`)
- Optional explicit start position (`S`)
- Actions: `N`, `E`, `S`, `W`
- **Wrap-around movement** at boundaries (toroidal topology)

The objective is to visit **every reachable free tile**.

This project addresses two tasks:

1. **CHECK PLAN (Plan Verification)**  
   Verify whether a given sequence of actions cleans the entire cave.

2. **FIND PLAN (Plan Synthesis)**  
   Generate an action sequence that guarantees full coverage.

---

## ✅ Task 1 — CHECK PLAN (Plan Verification)

### Goal
Given a grid and a move sequence, simulate the agent and determine:
- `GOOD PLAN` if all reachable free tiles are visited
- `BAD PLAN` plus coordinates of missed tiles otherwise

### Robustness handled
- Works with an explicit start cell (`S`)
- Also supports cases where the start position is **not specified**
- Prevents movement through walls
- Correctly simulates wrap-around movement

---

## 🧠 Task 2 — FIND PLAN (Plan Synthesis)

### Goal
Generate a plan that visits all reachable tiles.

### Approach (Classical Search)
- Model the cave as a **graph** of walkable cells
- Use **Depth-First Search (DFS)** to traverse all reachable nodes
- Add **backtracking moves** to ensure full coverage
- Handle both cases:
  - Start specified (`S`)
  - Start unspecified (plan must work regardless of start)

---

## 🎯 Skills Demonstrated
- Classical AI reasoning
- Graph modeling of grid-world environments
- DFS traversal + backtracking for coverage planning
- Plan simulation & verification
- Edge-case handling (unknown start, wrap-around)

---

## 📫 Contact
**Aleem Ud Din**  
Email: aleemjcs@gmail.com  
LinkedIn: https://linkedin.com/in/aleem-ud-din-56011021b/
