# AI Log, Audit Table & Reflection (Week 3)

## 1. Interpretation Auditor Table
| AI Claim / Sentence | Colour Code | How Verified / Checked | Verdict (Accepted / Rejected) |
| :--- | :--- | :--- | :--- |
| "The mean price is higher than the median across skewed items." | **Green** | Recomputed `mean()` and `median()` in Python; confirmed mean > median due to right-skewed outliers. | **Accepted** |
| "First-to-last percentage change shows an overall upward price shift." | **Green** | Recomputed `((last_price - first_price) / first_price) * 100` on chronological dates. | **Accepted** |
| "The gap between mean and median is likely caused by occasional supply bottlenecks." | **Amber** | Valid plausible explanation, though not directly proven by the price ledger alone. | **Accepted (as Explanation)** |
| "Consumers consistently paid the arithmetic mean price every week." | **Red** | False causal/typicality claim; extreme flagged spikes inflated the mean far above typical daily transactions. | **Rejected** |

---

## 2. Confused Classmate Transcript Excerpt
> **Classmate:** I still don't get it—the mean is literally the average, so why isn't it always the typical price?  
> **Me:** Because the mean adds every single price together and divides by the count. If nine days a staple costs Rs. 100, and on the tenth day a data error or rare spike makes it Rs. 1,000, the mean jumps to Rs. 190—a price nobody actually paid on any normal day.  
> **Classmate:** Okay, but why does the median stay unaffected?  
> **Me:** Because the median just lines all prices up from lowest to highest and picks the middle number. Even if the highest number jumps to Rs. 1,000 or Rs. 10,000, the middle position stays at Rs. 100, which reflects what a buyer actually pays on a typical day.  
> **Classmate:** Makes sense now! So when there are extreme spikes, the median tells the honest story of a normal day.

---

## 3. Reflection
- **Where my first draft said more than the data allowed:** In my pre-AI draft, I wrote a causal claim (`[C]`) stating that supply chain disruptions directly caused the price spikes. Looking closely at the data, the ledger only records prices and dates—it contains no supply chain columns, so claiming a specific external cause went beyond what the numbers proved.
- **Key Takeaway:** Always separate what the numbers strictly show (`[O]`) from possible real-world reasons (`[E]`), and verify every AI-generated number before reporting