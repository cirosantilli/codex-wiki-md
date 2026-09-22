<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x>0$, reflect a Brownian path after its first hitting of $x$. The [Strong Markov property](../../../../../../strong-markov-property.md) and symmetry preserve its law and exchange the events $\{S_1\geq x,\ B_1<x\}$ and $\{B_1>x\}$. The terminal equality event has [probability](../../../../../../probability.md) zero, so the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives

$$
\mathbb P(S_1\geq x)=2\mathbb P(B_1\geq x),\qquad
\mathbb P(S_1\leq x)=2\Phi(x)-1.
$$

Continuity of this distribution also gives no atom at zero. Therefore

$$
\boxed{\lim_{x\downarrow0}\frac{\mathbb P(S_1\leq x)}x=2\Phi'(0)=\sqrt{\frac2\pi}.}
$$

A useful global bound follows from the maximum of the standard [normal distribution](../../../../../../normal-distribution.md) density:

$$
\mathbb P(S_1\leq x)=2\int_0^x\frac{e^{-u^2/2}}{\sqrt{2\pi}}\,du\leq\sqrt{\frac2\pi}\,x\qquad(x\geq0).
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
