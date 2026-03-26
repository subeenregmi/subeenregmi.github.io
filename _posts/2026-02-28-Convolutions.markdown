---
layout: post
title:  "Convolutions"
date:   2026-02-28 14:56:08 +0000
tags: convolutions maths 
published: true 
---
The **convolution** of two functions $f$ and $g$ is defined as follows

$$
\large
(f * g)(t) = \int^{\infty}_{-\infty} f(\tau) g(t - \tau)\, d \tau
$$

in this blog post, we will explain what this formula means, what it visually represents and what we can do with it.

If you know integral calculus, you can sort of visualise what this definition really means.
- Firstly have $\tau$ which goes from $-\infty$ to $+\infty$ in really small steps $d\tau$ 
- $g(t - \tau)$ represents a shift of $g$ by $\tau$ along the $x$-axis
    - ($t - \tau$ also means that $g$ is flipped; but we will explain why this is needed later)
- $\int$ represents the area under the curve for $f(\tau) g(t - \tau)$

So what we are really doing is
1. Keeping $f$ still
2. Moving $g$ across the $x$ axis from $-\infty$ to $+\infty$ in really small steps
3. At each tiny step, we compute the total area under the curve upto that step - this value is the value of the convolution at that step

Here the the blue represents $f$ and red represents $g$, and the yellow is the convolution $f * g$  

![convolution visualisation](/assets/convolution.gif){:width="600" style="margin: auto; display: block;"}

{% comment %}

### Applying to 2D

Now what if our function $f$ represented an image?

{% endcomment %}
