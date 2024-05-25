---
layout: post
category: problem-solving
---

## Introduction
Here is my approach to problem 5 in *Iran MO 2023* (3rd Round.) **Always lots of fun!**

<p style="color: red">This is not a perfect solutions; it is my approach (brief solution), so there might be some logical loophole. Please let me know via comments :)</p>

Check out the problems at [here](https://artofproblemsolving.com/community/c3509728_2023_iran_mo_3rd_round)!

## Problem 2 (≤15')
Within seconds of reading the question, I became sure that the answer was **NO**. After a few tries, I figured out $$g(1)=f(1)=1$$, and I could make a key proposition

> $$g(n)$$ must be $$g(n) = n$$, which gives $$f(n)=2n-1$$, a contradiction.

I was stucked on trying to prove this proposition for a while. After about ten minutes, I realized I was hanging around to prove even though I already had a key idea. *Yuck!*

*Proof*. $$g(1)=1$$ (base condition). Assume that for $$1\leq k \leq n$$ $$g(k)=k$$. Then from $$ng(n)=(n-1)g(n-1)+f(n)$$, $$g(n)>\frac{(n-1)^2}{n}$$. Because $$g$$ is bijective, $$g(n)=n$$.

Thus, the proposition is correct and the answer is **NO**.

## Epilogue
