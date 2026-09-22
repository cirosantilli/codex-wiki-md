<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $F_n$ be the [distribution function](../../../../../../cumulative-distribution-function.md) of $X_n$. The limiting constant zero has [distribution function](../../../../../../cumulative-distribution-function.md) $F(x)=0$ for $x<0$ and $F(x)=1$ for $x\geq0$. For every $\varepsilon>0$, both $-\varepsilon$ and $\varepsilon$ are continuity points of $F$. Thus [convergence in distribution](../../../../../../convergence-in-distribution.md) implies $F_n(-\varepsilon)\to0$ and $F_n(\varepsilon)\to1$. Therefore

$$
0\leq\mathbb P(|X_n|>\varepsilon)
\leq F_n(-\varepsilon)+1-F_n(\varepsilon)\longrightarrow0.
$$

This proves

$$
\boxed{X_n\xrightarrow d0\ \Longrightarrow\ X_n\xrightarrow{\mathbb P}0.}
$$

The same proof after subtracting a fixed real $c$ proves [convergence in distribution to a constant implies convergence in probability](../../../../../../convergence-in-distribution-to-a-constant-implies-convergence-in-probability.md). A deterministic limit fixes the coupling automatically; the counterexample in (c) exploits a nonconstant limit whose [probability distribution](../../../../../../probability-distribution.md) alone does not fix that coupling.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
