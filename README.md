# Tiny is Mighty Enough Evaluating Tiny and Large Language Models for Controlling Autonomous Agents

## Associated Video
[![Alt Text](https://img.youtube.com/vi/IzUYMhG0nIs/0.jpg)](https://youtu.be/IzUYMhG0nIs)

### Table 2: User Prompts and Expected Responses — Panda Franka

| Task Number | Prompt | Response |
|---|---|---|
| 1 | Pick up cubeA and move it right | cubeA right |
| 2 | Pick up cubeA and move it left | cubeA left |
| 3 | Pick up cubeB and move it right | cubeB right |
| 4 | Pick up cubeB and move it left | cubeB left |
| 5 | Pick up cubeA and move it right three times | cubeA right right right |
| 6 | Pick up cubeA and move it right two times then pick up cubeB and move it left | cubeA right right cubeB left |
| 7 | Pick up cubeB and move it left then pick up cubeA and move it right two times then move cubeB right | cubeB left cubeA right right cubeB right |
| 8 | For this test you'll need to be able to pick up cubeA and move it left, after you are done moving cubeA left you need to pick up cubeB and move it right. | cubeA left cubeB right |
| 9 | For this test, start by shifting cubeA toward the left side. Once that's done, grab cubeB and slide it right a couple of times so it's roughly even with cubeA. | cubeA left cubeB right cubeB right |

---

### Table 3: Task Results — Panda Franka

| Models | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | Total Score |
|---|---|---|---|---|---|---|---|---|---|---|
| TinyLlama | 1 | 1 | 1 | 1 | 0 | 0 | 0 | 1 | 0 | 5 |
| DeepSeek-R1 (1.5B) | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 1 |
| Gemma-2 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 1 | 0 | 7 |
| Phi-2 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 8 |
| DeepSeek-R1 (7B) | 1 | 1 | 0 | 0 | 1 | 0 | 0 | 1 | 0 | 4 |
| Llama 3.1 (8B) | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 1 | 1 | 9 |
| GPT-4o-mini | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 9 |
| GPT-4o | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 1 | 1 | 8 |

---

### Table 4: User Prompts and Expected Responses — Frozen Lake

| Task ID | Prompt | Response |
|---|---|---|
| 1 | Go right | right |
| 2 | Go left | left |
| 3 | Go Up | up |
| 4 | Go Down | down |
| 5 | Go right three times | right right right |
| 6 | Go right then down then right again | right, down, right |
| 7 | Go right four times then left two times and down once | right, right, right, right, left, left, down |

---

### Table 5: Task Results — Frozen Lake

| Models | 1 | 2 | 3 | 4 | 5 | 6 | 7 | Total Score |
|---|---|---|---|---|---|---|---|---|
| TinyLlama | 1 | 1 | 1 | 1 | 1 | 0 | 0 | 5 |
| DeepSeek-R1 (1.5B) | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 7 |
| Gemma-2 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 7 |
| Phi-2 | 0 | 0 | 1 | 1 | 1 | 1 | 1 | 5 |
| DeepSeek-R1 (7B) | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 7 |
| Llama 3.1 (8B) | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 7 |
| GPT-4o-mini | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 7 |
| GPT-4o | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 7 |

---

### Table 6: User Prompts and Expected Responses — Lunar Landing

| Task Number | Prompt | Response |
|---|---|---|
| 1 | Go right | right |
| 2 | Go left | left |
| 3 | Go Up | up |
| 4 | Go right two times, then do nothing, then go up | right, right, nothing, up |
| 5 | Go right, go left, then do nothing two times, then go up | right, left, nothing, nothing, up |

---

### Table 7: Task Results — Lunar Landing

| Models | 1 | 2 | 3 | 4 | 5 | Total Score |
|---|---|---|---|---|---|---|
| TinyLlama | 1 | 1 | 1 | 0 | 0 | 3 |
| DeepSeek-R1 (1.5B) | 1 | 1 | 1 | 1 | 1 | 5 |
| Gemma-2 | 0 | 0 | 1 | 1 | 1 | 3 |
| Phi-2 | 1 | 1 | 0 | 0 | 0 | 2 |
| DeepSeek-R1 (7B) | 0 | 1 | 1 | 1 | 1 | 4 |
| Llama 3.1 (8B) | 1 | 1 | 1 | 1 | 1 | 5 |
| GPT-4o-mini | 1 | 1 | 1 | 1 | 1 | 5 |
| GPT-4o | 1 | 1 | 1 | 1 | 1 | 5 |

---

### Table 8: User Prompts and Expected Responses — Reacher

| Task Number | Prompt | Response |
|---|---|---|
| 1 | Swing right | right |
| 2 | Swing left | left |
| 3 | Swing right two times then center | right, right, center |
| 4 | Swing left two times then center then swing right | left, left, center, right |
| 5 | Start by swinging the arm to the right, then bring it back to the left twice before returning it to the center position to finish. | right, left, left, center |
| 6 | If the arm isn't centered, swing it left first. After that, swing to the right two times and finally center it again when you're done. | left, right, right, center |

---

### Table 9: Task Results — Reacher

| Model | 1 | 2 | 3 | 4 | 5 | 6 | Total Score |
|---|---|---|---|---|---|---|---|
| TinyLlama | 0 | 1 | 0 | 0 | 1 | 0 | 2 |
| DeepSeek-R1 (1.5B) | 1 | 1 | 1 | 1 | 1 | 1 | 6 |
| Gemma-2 | 1 | 1 | 1 | 1 | 1 | 0 | 5 |
| Phi-2 | 0 | 0 | 1 | 0 | 1 | 0 | 2 |
| DeepSeek-R1 (7B) | 1 | 1 | 1 | 0 | 1 | 1 | 5 |
| Llama 3.1 (8B) | 1 | 1 | 1 | 1 | 1 | 1 | 6 |
| GPT-4o-mini | 1 | 1 | 1 | 1 | 1 | 1 | 6 |
| GPT-4o | 1 | 1 | 1 | 1 | 1 | 1 | 6 |

---

### Table 10: User Prompts and Expected Responses — Mountain Car

| Task Number | Prompt | Response |
|---|---|---|
| 1 | Go right | right |
| 2 | Go left | left |
| 3 | Go right six times | right, right, right, right, right, right |
| 4 | Go right three times than go left six times | right, right, right, left, left, left, left, left, left |

---

### Table 11: Task Results — Mountain Car

| Model | 1 | 2 | 3 | 4 | Total Score |
|---|---|---|---|---|---|
| TinyLlama | 0 | 0 | 0 | 0 | 0 |
| DeepSeek-R1 (1.5B) | 1 | 1 | 1 | 0 | 3 |
| Gemma-2 | 1 | 1 | 1 | 1 | 4 |
| Phi-2 | 1 | 1 | 1 | 0 | 3 |
| DeepSeek-R1 (7B) | 1 | 1 | 1 | 1 | 4 |
| Llama 3.1 (8B) | 1 | 1 | 1 | 1 | 4 |
| GPT-4o-mini | 1 | 1 | 1 | 1 | 4 |
| GPT-4o | 1 | 1 | 1 | 1 | 4 |

---

### Table 12: User Prompts and Expected Responses — Car Racing

| Task Number | Prompt | Response |
|---|---|---|
| 1 | Go forward | forward |
| 2 | Go right | right |
| 3 | Go left | left |
| 4 | Go forward two times than take a left | forward, forward, left |
| 5 | Go forward six times then take a left two times than go forward four more times | forward, forward, forward, forward, forward, forward, left, left, forward, forward, forward, forward |

---

### Table 13: Task Results — Car Racing

| Model | 1 | 2 | 3 | 4 | 5 | Total Score |
|---|---|---|---|---|---|---|
| TinyLlama | 0 | 0 | 0 | 0 | 0 | 0 |
| DeepSeek-R1 (1.5B) | 1 | 1 | 1 | 0 | 0 | 3 |
| Gemma-2 | 1 | 1 | 1 | 0 | 0 | 3 |
| Phi-2 | 0 | 0 | 0 | 0 | 0 | 0 |
| DeepSeek-R1 (7B) | 1 | 1 | 1 | 1 | 1 | 5 |
| Llama 3.1 (8B) | 1 | 1 | 1 | 1 | 1 | 5 |
| GPT-4o-mini | 1 | 1 | 1 | 1 | 1 | 5 |
| GPT-4o | 1 | 1 | 1 | 1 | 1 | 5 |

---

### Table 14: Total and BiPaN Scores

| TinyLlama | DeepSeek-R1 (1.5B) | Gemma-2 | Phi-2 | DeepSeek-R1 (7B) | Llama 3.1 (8B) | GPT-4o-mini | GPT-4o |
|---|---|---|---|---|---|---|---|
| 15 | 25 | 29 | 20 | 29 | 36 | **36** | 35 |
| 13.64 | **16.67** | 14.50 | 7.41 | 4.14 | 4.50 | 4.50 | 0.18 |

---

### Table 15: Average Time (seconds) to Run 100 Prompts

| Models | Panda | Frozen Lake | Lunar Land. | Reacher | M. Car | Car Race. | Avg |
|---|---|---|---|---|---|---|---|
| TinyLlama | 0.31 | 0.52 | 0.24 | 0.53 | 0.39 | 0.50 | 0.41 |
| DeepSeek-R1 (1.5B) | 2.30 | 2.04 | 2.82 | 2.63 | 3.69 | 2.66 | 2.69 |
| Gemma-2 | 0.31 | 0.28 | 0.28 | 0.25 | 0.28 | 0.29 | **0.28** |
| Phi-2 | 1.06 | 0.87 | 0.61 | 0.51 | 1.08 | 0.26 | 0.73 |
| DeepSeek-R1 (7B) | 6.42 | 4.97 | 5.71 | 6.33 | 9.38 | 6.77 | 6.60 |
| Llama 3.1 (8B) | 0.35 | 0.30 | 0.31 | 0.29 | 0.33 | 0.31 | 0.31 |
| GPT-4o-mini | 0.70 | 0.73 | 0.79 | 0.59 | 0.62 | 0.73 | 0.69 |
| GPT-4o | 0.75 | 0.64 | 0.62 | 0.63 | 0.64 | 0.74 | 0.67 |
