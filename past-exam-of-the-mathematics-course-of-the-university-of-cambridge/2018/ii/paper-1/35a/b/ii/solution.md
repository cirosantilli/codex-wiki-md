<h1 id="35a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Because increasing the length by $dL$ requires work $f dL$ on the chain, its [first law of thermodynamics](../../../../../../../first-law-of-thermodynamics.md) is

$$
dE=T dS+f dL.
$$

All configurations have the same energy, so at fixed $E$ and $N$,

$$
f=-T\left(\frac{\partial S}{\partial L}\right)_{E,N}.
$$

Differentiating the entropy found above gives

$$
\frac{\partial S}{\partial L}
=\frac{k_B}{2a}\log\frac{1-L/(Na)}{1+L/(Na)},
$$

and hence the [entropic Hooke law for a one-dimensional chain](../../../../../../../entropic-hooke-law-for-a-one-dimensional-chain.md) is

$$
\boxed{f=\frac{k_BT}{2a}\log\frac{1+L/(Na)}{1-L/(Na)}
=\frac{k_BT}{a}\operatorname{artanh}\frac{L}{Na}.}
$$

When $L\ll Na$, the [Taylor expansion](../../../../../../../taylor-expansion.md) of $\operatorname{artanh}x$ gives

$$
\boxed{f\sim\frac{k_BT}{Na^2}L,}
$$

which is [Hooke's law](../../../../../../../hooke-s-law.md). Conversely, at fixed force,

$$
\boxed{L=Na\tanh\frac{fa}{k_BT}.}
$$

The extension decreases as the temperature rises and tends to zero as $T\to\infty$: the rubber contracts on heating at fixed tension.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [35A](../../../35a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
