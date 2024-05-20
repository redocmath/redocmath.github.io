---
layout: post
category: problem-solving
---

## Introduction
Here are my approaches to *Tournament of Towns 2023/2024* (Fall 2023, Senior A-level.) I've heard a lot about *Tournament of Towns*, but this is my first try to solve problems in *Tournament of Towns*. I recorded time taken to solve each problem, to express how that problem was difficult for me.

Check out the problems at [here](https://artofproblemsolving.com/community/c3683569_20232024_tournament_of_towns)!

## Problem 1 (≤5')
After I read this problem, I was almost sure that the answer must be *equal*. In detail, I believed there must be a way to *pair* two roots completely. Fortunately, it was not so hard to find the way.

Let 
\\[
p_{(a_0, a_1, ..., a_{45})}(x) = \sum_{0\leq i\leq45} a_i x^i
\\]
and
\\[
X_{(a_0, a_1, ..., a_{45})} = \lbrace x~\vert~ p_{(a_0, a_1, ..., a_45)}(x)=0 \rbrace
\\]
where $$a_i \in \left\{1,2,...,46\right\}$$. Then, we can easily show 
\\[
\forall x\in X_{(a_0, a_1, ..., a_{45})}\quad x<0.
\\]
Also, it is trivial that
\\[
\left\lbrace\frac1x \vert x \in X_{(a_0, a_1, ..., a_{45})}\right\rbrace = X_{(a_{45}, a_{44}, ..., a_0)}.
\\]
Because $$\left\lbrace x+1, \frac1x+1 \right\rbrace = \left\lbrace positive, negative \right\rbrace$$ for $$x<0$$, 

\\[
\left\vert\left\lbrace x \vert x\in X_{A} \cup X_{A^{-1}} \wedge x+1>0\right\rbrace\right\vert = 
\left\vert\left\lbrace x \vert x\in X_{A} \cup X_{A^{-1}} \wedge x+1<0\right\rbrace\right\vert
\\]

where $$A=(a_0, a_1, ..., a_{45})$$ and $$A^{-1}=(a_{45}, a_{44}, ..., a_0)$$. Obviously for every $$A$$ we can find $$A^{-1}\neq A$$, the answer must be *equal*.

## Problem 2 (20')
I tried to solve smaller problem first, so I generalized the numeral system and observed $$N$$ from unary to ternary by hand. Let $$N(d)$$ be $$N$$ for $$d$$-base numeral system.

\\[
{\lbrace N(d)\rbrace}_{d=1}^3 = \lbrace1,3,7\rbrace = \lbrace2^1-1, 2^2-1, 2^3-1\rbrace
\\]

From observation, I guessed $$N(d)$$ would be $$2^d-1$$.

*Proof.* $$N(1)=2^1-1$$ (base condition). Let's assume $$N(d)=2^d-1$$ and show $$N(d+1)=2^{d+1}-1$$ to apply mathematical induction. We can easily show $$N(d+1)\geq 2N(d)+1=2^{d+1}-1$$ with a constructive solution:

\\[
X(d+1) = X(d)\circ(d+1)\circ X(d)
\\]

where $$X(d)$$ is one of the possible number whose length is $$N(d)$$ and $$\circ$$ is concatenation. Now let's show $$N(d+1)\leq 2N(d)+1$$. Obviously 

\\[
\left\vert\left\lbrace X(d+1)_i \in \lbrace1,2,...,d\rbrace \right\rbrace\right\vert \leq N(d)
\\]

and

\\[
\left\vert\left\lbrace X(d+1)_i = (d+1) \right\rbrace\right\vert \leq N(d)+1
\\]

because there must not be adjacent digits $$(d+1)$$. These two inequalities easily prove $$N(d+1)\leq 2N(d)+1$$. Finally, $$N(d+1)=2N(d)+1 \Rightarrow N(d)=2^{d}-1$$.

## Problem 3 (15')

## Problem 4

## Problem 6

## Problem 7

## Epilogue

Since I was young, I have been afraid of geometry problems. And it has leaded me to avoid to solve geometry problems. 


![Geometry Meme](https://images2.memedroid.com/images/UPLOADED27/51a6caa51e932.jpeg)

Recently, however, I realized my terrible geometrical skills and started to try more geometry problems rather than avoiding them. I feel proud of myself because I solved Problems 4 and 5 at this time, and this is why problem-solving is more meaningful for me—**impressive and fun**.


