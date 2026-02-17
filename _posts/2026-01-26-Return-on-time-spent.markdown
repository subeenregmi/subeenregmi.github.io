---
layout: post
title:  "Leveraging tech debt to move faster"
date:   2026-01-26 21:58:08 +0000
tags: technical software-engineering 
---

Solutions to a given problem can be evaluated by two metrics: the **value/effectiveness** of the solution and the **time** it took to create it. 
By plotting these two metrics against each other, we usually get a graph that looks something like this:

![time value graph](/assets/time-value-graph.png){:width="500" style="margin: auto; display: block;"}

**Momentum** is the concept of "how fast can we get this feature in", defined by value / time, I believe it is the single metric that all engineers should optimize for.
It is influenced by most other factors, for example: 
- your social skills - how well can you sell going from X to Z?
- your programming abilities - how well can you convey you are actually going from X to Z?
- your rationale - what does going from X to Z do for and against you?

By optimizing for momentum, we get several benefits:
- faster updates, releases and changes
- accelerated developer learning and team growth
- faster product feedback cycles

Not only do we increase speed, we also increase **our confidence in strategic play**. 
Inherent risks decrease, experimentation seems necessary and barriers and blocks are broken. 
We are given freedom to test what works and what sticks, and an environment that allows for this is an environment that invites an excellent engineering culture.

However when increasing momentum, there is a natural increase **tech debt**. 
This represents all the menial lingering tasks, the stuff that we push to the side and promise to do later and never do. 
The tasks that end up blocking you from making that change and makes you wonder why it was not done sooner.

Often it is seen in a negative light, as seen in this picture:

![tech debt](/assets/evil-tech-debt.png){:width="500" style="margin: auto; display: block;"}

However I believe in when strategically leveraging, managing and monitoring levels of tech debt it can help us tremendously in the pursuit of momentum.

Let's say a customer wants a feature X that is in the feature space S (the realm of related possible features to X), we could:
1. Write a change that provides feature X
2. Write a longer change that provides support to features in S and then provide feature X

What is the right answer? 
- Option 1 is fast and direct, increasing momentum now and establishing a good customer experience but leaving us exposed to tech debt if we chose to add more features in S. 
- Option 2 is more methodical but slow, providing a solution that increases momentum when adding more features in S, but can be dangerous to customer relations.

This is where we come and think:
- Do we think we are going to add more features from S?
    - When? In a week?, a month?, a year?
    - How much features would we add?
        - Are there a small amount of features that generate the highest return?
    - Have potential/current customers asked for features in S?
- Do we think feature X will change much?
- Are losing out on working on better things if we choose to add feature support for S?
- Are there any structural changes required for both options?
    - New database, cache, etc.
    - Are the any new relevant costs? (cloud, storage, etc.)
    - How much people will I need to talk to this about?
- Who should be on a task like this?
    - Is this task suitable for a junior/mid-level engineers?
- How big is option 1 relative to option 2?
- How is the relationship between customer and us?
    - Can a delay potentially harm this customer relationship?
- Is there already existing tech debt to do for X?

By questioning the nature of this tech debt, we can achieve a much better momentum evaluation for both options. 
We also develop a good sense confidence of confidence in the chosen option, so when questions come (and they do come) you are ready to answer with a thought out answer.

Tech debt is not bad, unmanaged tech debt is.
Leveraging tech debt strategically allows you to evaluate and prioritize momentum, doing so will not only make you a great engineer - it will give a more proven, logic-driven framework that can be applied in all domains.
