<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Given an output $y$ of positive [probability](../../../../probability.md), the ideal observer chooses a symbol maximizing the posterior:

$$
\boxed{g(y)\in\operatorname*{arg\,max}_{x\in A}P(X=x\mid Y=y).}
$$

Ties may be broken arbitrarily, and the choice at an impossible output does not matter. This is [maximum a posteriori decoding](../../../../maximum-a-posteriori-decoding.md). It minimizes conditional error at each $y$, because a deterministic decision $x$ is correct with [probability](../../../../probability.md) $P(X=x\mid Y=y)$; a randomized decision is a weighted average of these success probabilities and cannot exceed their maximum.

Write $\Pi_y=\max_xP(X=x\mid Y=y)$. Then $w(y)=1-\Pi_y$. Applying the two cases from part (b) to the posterior distribution gives

$$
H(X\mid Y=y)\geq2(1-\Pi_y)=2w(y).
$$

Average with respect to the output law to obtain the [conditional entropy upper bound on minimum decoding error](../../../../conditional-entropy-upper-bound-on-minimum-decoding-error.md):

$$
\boxed{\mathbb Ew(Y)\leq\frac12H(X\mid Y).}
$$

This is an upper bound on the optimum error [probability](../../../../probability.md); it does not hold for arbitrary deliberately poor decoding rules.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
