<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Conditioning on the epoch length gives the [probability generating function](../../../../../../probability-generating-function.md)

$$
\mathbb E[s^{Y_j}\mid T_j]=\exp\left[-\frac{j\theta}{2}(1-s)T_j\right].
$$

The [Laplace transform of an exponential distribution](../../../../../../laplace-transform-of-an-exponential-distribution.md) then yields

$$
\mathbb E[s^{Y_j}]=\frac{\binom j2}{\binom j2+(j\theta/2)(1-s)}=\frac{j-1}{j-1+\theta(1-s)}=\frac{p_j}{1-(1-p_j)s},\qquad p_j=\frac{j-1}{j-1+\theta}.
$$

This is the [geometric mutation count in a coalescent epoch](../../../../../../geometric-mutation-count-in-a-coalescent-epoch.md). With the zero-based [geometric distribution](../../../../../../geometric-distribution.md) convention,

$$
\boxed{P(Y_j=k)=p_j(1-p_j)^k,\qquad k=0,1,\ldots.}
$$

At $\theta=0$, this reduces to $Y_j=0$ almost surely.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
