
---

## 🧩 Architecture

![diagram](upscaiagent1.png)

---
1)  Text Feedback
2)  Generate a score 0-10

Iske baad by all 3 nodes value will be move to final evolution node ke pass
![[upscaiagent2.png]]
3 nodes se text feedback arha hai usse we will make summarize feedback karege
also it will inclue the score from all the 3 nodes get the average of the nodes

I dont like the notes styling and view of the notes 

## 🧠 Workflow Logic

- Generate **text feedback**
- Assign a **score (0–10)**

---

## 🔁 Parallel Evaluation

All 3 nodes:
- COT LLM
- DOA LLM
- Language LLM

➡️ Send results to **Final Evolution Node**



---
> [!info] INFO — Parallel Evaluation
> All 3 LLM nodes run simultaneously. Final Evolution Node aggregates using weighted average.

| NODE | WEIGHT | LAST SCORE | STATUS |
|------|--------|------------|--------|
| cot_llm | 0.40 | 7.8 | active |
| doa_llm | 0.35 | 7.1 | active |
| language_llm | 0.25 | 7.2 | testing |

> [!success] SUCCESS — Last Run
> avg_score: 7.4 / 10  ·  latency: 1.2s  ·  tokens: 3,840


```Python
print("hellow
if a in 10: 
	print(sd)
```



