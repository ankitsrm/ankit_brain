
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

# State 

in state we need to keep what all variable 
```
essay_text
cot_feedback
doa_feedback
language_feedback
summarized_feedback
final_feedback
individual_score (List hoga 3 value store karege)
average(float)
```

- Why we need <mark style="background: #ABF7F7A6;">reducer function</mark>
	as 
