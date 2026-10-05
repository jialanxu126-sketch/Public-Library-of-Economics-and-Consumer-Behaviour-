---
layout: research
title: "How agentic AI deploys human heuristics as a surrogate consumer"
category: "Behavioural Economics · Consumer Behaviour · AI Commerce"
description: "How AI shopping agents respond to pricing cues, information costs and the specificity of the instructions they receive."
audience: "Businesses · AI shoppers · AI developers"
reading_time: "15 min"
---

## Understanding
Understand:
AI shopping agents are gaining popularity, and these researchers wanted 
to know whether they would behave like humans when presented with popular 
marketing strategies  such as just-below pricing (for instance pricing 
something at $9.99 instead of $10) or promotional discounts (for example:
20% off). AI agents were tested in an experimental sandbox called Tool-lab 
in which researchers observed how the agent thinks when deciding on the 
most suitable product. However, the agent was not given all product 
information initially, and to access additional information, the bot must 
pay a cost (these were variables like computing power time or API fees). 
They tested 8 major AI models across 16400 shopping sessions changing the 
cost for the AI agent to research and how specific the human prompt was.


### Study 1

Researchers created 1014 coffee shopping scenarios where the best choice is 
already calculated, then changed the cost of accessing the information and 
the specificity of the user’s instructions. This allowed them to test whether 
AI agents would make similar shortcuts to human shoppers.
They also tested the change in AI’s behaviour when purchase volume increased.


<details class="research-details">
<summary>Variables</summary>

<div class="Independent variables">
1. Cost for the bot to research and access more information about the product.
2. Specificity of human prompt of a vague prompt like: find the best deal, vs 
  a detailed prompt like: find the lowest price per ounce.
3. AI model type (Gemini 3.5 Flash Lite, Gemini 3.8 Flash, Gemini 3.1 Pro, 
  GPT 5.6 Luna, GPT 5.6 Terra, GPT 5.6 Sol, Claude Sonnet 5, and Opus 5). 
4. Price layout in dollars vs in cents
5. Purchase volume (1, 5, 50 and 250 bags of coffee)

</div>

<div class="Dependent variables">
1. How detailed or thorough the AI agent’s research was into the products.
2. What the AI searched for such as things like price and weight.
3. Whether the AI bought the best financial deal or whether it made a mistake.
</div>

<div class=“Control variables”>
1. Simulation store environment (Tool-Lab)
2. Difficulty in calculations for the AI agent when finding the best deals.
3. They compared all results against one normative objective optimiser (an 
  algorithm that always finds the absolute best course of action).

</details>


### Key findings

Results:
The layout of pricing made no difference to the bot’s behaviour and ⅞ models 
did not fall for pricing strategies. With Gemini Flash as the only one who 
focused more on the dollar digits.
When that AI agent was given a precise instruction, the cost of data no longer 
had an effect on its performance.
However, with vague instructions and a high data cost, the bot only looked at 
one of 2 variables needed to find the best deal, and therefore its performance 
was suboptimal (deficient)
When purchase volume increased under a vague prompt but all information was open, 
the bot’s accuracy decreased dramatically, with only Gemini Flash staying 
consistent. 


### Study 2

Study 2 tested how well LLMs calculate value when products are on promotional discounts. 
They were given 4 different coffee options, half with random discounts and were told to 
calculate the best unit price.


<details class="research-details">
<summary>Variables</summary>

<div class="Independent variables">
1. Original price of coffee before discounts
2. Discount applied to coffee (ranging from 5-40% in 5% increments)
3. Dollar value saved by discount
4. Product weight 
</div>

<div class="Dependent variables">
1. the product chosen by the LLM
</div>

<div class=“Control variables”>
1. Brand options (McCafé, Maxwell House, Starbucks and Folgers)
2. Every test featured 4 options to choose from
3. 50% of options were assigned a random discount
4. How much information was accessible to the LLM
</details>


### Key findings

Results:
All 8 LLMs behaved logically at a basic level where they selected the 
lower base price, higher discounts and more weight to dollar ratio. 
However, when researchers tested whether LLMs viewed $1 discount equally 
to a $1 cheaper price for instance: $10, now $8 vs just $8 original price; 
6 out of 8 LLMs passed the test perfectly however, Opus showed a sale bias 
where it fell for the marketing trick. Flash Lite on the other hand, 
undervalued discounts.



## Connect

Connect
The results from this study can be useful in several ways. With over 69% of 
consumers using AI as shopping assistants in the US with growing frequency 
(CSA, 2026), businesses should consider tailoring online site designs or 
information layout to AI shoppers. AI agents can sometimes behave similarly 
to humans in decision making, which suggest that businesses need to adapt and 
design marketing strategies differently when a LLM is acting as the consumer.

<details class="Relevance to:">

<div class="Businesses”>
- When using AI agents for procurement or competitive research, eliminate vague 
  prompts to ensure the algorithm does not overlook key details.
- As the study has shown, an AI agent's accuracy to select your product would 
  decrease when purchase volume increases. To encourage your product to be selected, 
  display the lowest unit price prominently.
- Traditional pricing techniques may become less reliable with an AI shopper than a 
  human, although this study did not state their ineffectiveness, it is important to 
  understand their diminished impact.
- Opus showed a bias towards discounted products in the experiment, therefore 
  businesses whose customers increasingly use AI shopping agents can consider how 
  promotional pricing is interpreted by these systems.
</div>

<div class=“Consumers”>
- To conduct the most successful search with a LLM, use specific prompts that obliges 
  the machine to search thoroughly.
- Do not trust the AI agents’ recommendations blindly, especially with in-bulk orders.
- Use the model that performed best for your search.
</div>

<div class=“AI agent developers”>
- Since AI agents are currently vulnerable to vague prompts, developers could consider 
  designing systems that ask consumers to clarify instructions.
</div>
  
</details>
## Analysis
Analysis:
This study provides us with an insight into the changing landscape of online shopping. 
AI agents are generally less susceptible to some traditional marketing techniques than humans, 
however, it still depends heavily on the instructions they are given. This suggests that AI 
may not simply be a replacement for the human consumer, instead it may introduce a new 
category of decision-makers for businesses to understand.

One key limitation to consider is that their results are based on what the LLM did rather than 
why it did so, which can diminish our understanding of the way it acts in order to change it. 
This study showed us what AI agents behave in controlled environments but not why they did so. 
A decision similar to human heuristics does not necessarily mean that they process information 
the same way humans do psychologically. If they think differently to humans, then marketing 
strategies designed originally for humans may not have the same effect on AI agents, therefore 
business must understand how these agents search, prioritize and interpret information rather 
than assuming the same psychology applied to humans would apply to them.

Future research could test more subjective products like clothing, fragrance or sports equipment 
etc, where there may not be an objectively optimal choice as it depends heavily on personal 
preference, in such scenarios, it may reveal how LLMs prioritise value, aesthetic and functionality 
when there is no “best” choice. It would also be useful to test more realistic shopping scenarios 
that involve factors like delivering time, scarcity or trustworthiness; this can reveal whether 
the patterns observed in this study change across other scenarios when the AI agent must weigh 
multiple factors rather than simply calculating the best mathematical choice.


## Sources

Sources:
