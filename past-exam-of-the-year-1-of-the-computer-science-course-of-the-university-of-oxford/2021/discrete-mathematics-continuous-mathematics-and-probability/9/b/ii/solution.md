<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $t_i=\mathbb E_i[X]$. Time is accumulated in each transient chamber before the next move; arrival at either terminal state ends the trial immediately. Thus $t_0=t_k=0$. A block of $k$ identical rightward choices forces absorption, so the [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md) gives finite [expected value](../../../../../../expected-value-split.md) of $X$.

[First-step analysis](../../../../../../first-step-analysis.md) now gives

$$
t_i=1+\tfrac12t_{i-1}+\tfrac12t_{i+1},\qquad1\leq i\leq k-1.
$$

The quadratic $t_i=i(k-i)$ has the correct boundary values and second difference $t_{i+1}-2t_i+t_{i-1}=-2$, so it solves this system. The difference of two solutions would be linear in $i$ with zero values at both endpoints, hence zero. Therefore

$$
\boxed{\mathbb E_i[X]=i(k-i)\text{ minutes}.}
$$

This is the [expected duration of symmetric gambler's ruin](../../../../../../expected-duration-of-symmetric-gambler-s-ruin.md). It includes the first minute in the starting transient chamber and does not add a minute after absorption.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
