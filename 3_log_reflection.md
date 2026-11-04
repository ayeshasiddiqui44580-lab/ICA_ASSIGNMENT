AI flagged my claims with the following response:
I’ve read the handout and your attempt. I’ll only question and push here. Rewriting your questions is your job.

Claim 1: “prices are increasing”

Which prices? Your question talks about “the prices” as if one number exists. What would you need to decide before you could compute a single rate?
You named “percentage change over a period”, but that’s a formula, not a variable. Which raw columns does it need, and which dates would you compare?
If prices went up in week 2 and then stayed flat, would “prices are rising” be true? How many time points do you need before you’d say so?

Claim 2: “prices rise at different rates in different cities”

Your claim is about different rates of increase, but your example and your question are about different levels. Are those the same claim? Could Islamabad be higher in level and rising more slowly than Karachi? Which one does your question actually test?
“General price level” means a basket of goods. If cities sell items in different units or quantities, how would you compare them fairly?
Your example names two specific cities. What do you assume about which cities the data covers, and what happens to your question if that assumption fails?

Your predictions

In the handout, “shape” means rows × columns, but you also predicted skew. Skew of which variable, and what about a price column would make it right-skewed?
You predicted 5 dates and 8 items, and also 96 rows. Multiply 5 × 8, then compare that to 96. What does the gap say about your mental model of the dataset?
“Seven columns should be evaluating the rate of price change” is unclear. Do you mean columns in the file or columns you’d compute? If the file doesn’t have them, what would you derive them from?
If 96 and “five columns” came from anywhere other than your head, say so in the snapshot. The handout wants predictions made before running any code.

What the data cannot say
Suppose you answered both questions perfectly. What would still be unanswerable? Think about the headline claims in the handout, such as “out of reach” and “just spend differently”. What data would they need that prices alone don’t give you?

to which i replied with:
claim 1 related answers:
average price is to be taken and a percentage change over a period of time basically is the rate (which is the variable) calculated chronologically. 

claim 2 related answers:
different rates of increase in the price level is what my question is testing. 
a basket of good will need to have one standardized per unit price which are matched across cities/regions for this calculation. 
if this assumption fails to be proven, it simply is proven wrong. 

answers related to my predictions:
i believe it is a rightly skewed distribution since the mean leans more towards the max than the min and is greater than the median. 
the two additional columns would be the ones i compute for a critical analysis which the current data doesnt provide.
_________________________________________________________________________________________
you may ignore the text mentioned above this, they're for submission in the AI_log.md file, now i would like you to propose five alternative questions. 

the five questions proprosed by AI were:
Here are five alternative questions. I haven’t marked which ones the data can support, and I haven’t picked one for you.

From each item’s first observation to its last, what is its percentage price change, and do all items move in the same direction?
For the same item, is the price gap between two cities constant over time, widening, or narrowing?
Which item contributes most to the change in an average price level, and does that change if items are weighted by how much households actually buy?
Do prices rise steadily from period to period, or in a few sudden jumps?
Are staple goods becoming less affordable relative to household incomes in one city compared with another?

i ended up using q1,2 and 4 from AI and my own two claims since incomes and weighted indexes (or the proportion of income spent on said items) were not provided which led to the elimination of q3 and 5. 

REFLECTION:
Across 12 weeks, average prices rise in both cities: City 1 increases 12.9% and City 2 increases 12.5%. Individual items vary, from Pulse C’s 3.75% to Sweetener D’s 19.80% increase in City 1.
City 2 consistently costs Rs 6 more per item than City 1, while City 1 experiences slightly higher percentage increases. Average price increases differ by only 0.4 percentage points.
The dataset cannot establish actual geographical differences because cities are anonymous. It is illustrative teaching data, not real-world evidence. Missing household incomes also prevent affordability analysis.
Prices rise relatively steadily, rather than through sudden jumps, although individual items fluctuate between observations. City 1’s average weekly increases range approximately from 0.79% to 1.54%, demonstrating gradual progression.  
Question 5, concerning whether staple goods are becoming less affordable relative to household incomes, was the most tempting suggestion. It directly addresses the original concern about prices becoming “out of reach” and connects price increases to people's actual living conditions. However, it is unsupported because the dataset contains no household income information, making it impossible to measure affordability or determine whether purchasing these goods has become financially more difficult.
