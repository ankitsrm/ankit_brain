
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

# 🎨 6. Make it look like REAL dashboard (CSS)

Add this to your snippet:

```css id="c5ovh1"
/* Dashboard tables */
table {
  border-radius: 10px;
  overflow: hidden;
  border: 1px solid rgba(255,255,255,0.08);
}

/* Status colors */
td {
  font-weight: 500;
}

/* Highlight unhealthy */
td:contains("degraded"),
td:contains("failed") {
  color: #ff6b6b;
}

/* Highlight healthy */
td:contains("healthy") {
  color: #51cf66;
}

/* Card feel */
.markdown-preview-view {
  background: #0b0f14;
}