<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [Black-Scholes model](../../../../../../black-scholes-model.md),

$$
S_t=S_0\exp\!\left(\sigma W_t-\frac12\sigma^2t\right).
$$

Conditioning on $\mathcal F_t$ and using the [moment-generating function](../../../../../../moment-generating-function.md) of the independent Gaussian increment $W_T-W_t$ gives

$$
C_t=\sqrt{S_t}\exp\!\left(-\frac18\sigma^2(T-t)\right)
=c(t,S_t).
$$

The function $c$ satisfies the zero-rate [Black-Scholes equation](../../../../../../black-scholes-equation.md), so [Itô formula](../../../../../../ito-s-lemma.md) leaves only its stochastic term:

$$
dC_t=\partial_sc(t,S_t)\,dS_t.
$$

Consequently the required [delta hedge](../../../../../../delta-hedge.md) is

$$
\boxed{\Delta(t,s)=\partial_sc(t,s)
=\frac1{2\sqrt s}\exp\!\left(-\frac18\sigma^2(T-t)\right).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
