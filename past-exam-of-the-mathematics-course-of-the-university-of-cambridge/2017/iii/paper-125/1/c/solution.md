<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\pi$ be the [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) and let $a=p+1-N$ be its [Trace of Frobenius](../../../../../../trace-of-frobenius.md). Its characteristic equation is $\pi^2-[a]\pi+[p]=0$, so the [trace of the square of an elliptic-curve endomorphism](../../../../../../trace-of-the-square-of-an-elliptic-curve-endomorphism.md) is $a^2-2p$. The [elliptic-curve point count over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md) therefore gives

$$
\#E(\mathbb F_{p^2})=p^2+1-(a^2-2p)
=(p+1)^2-(p+1-N)^2.
$$

The [prime-square point-count formula](../../../../../../prime-square-point-count-formula.md) is consequently

$$
\boxed{\#E(\mathbb F_{p^2})=N\bigl(2p+2-N\bigr).}
$$

One can also obtain it directly from the [degree of an isogeny](../../../../../../degree-of-an-isogeny.md): the maps $1-\pi$ and $1+\pi$ are [separable isogenies](../../../../../../separable-isogeny.md), with degrees $p+1-a$ and $p+1+a$. Their composition is $1-\pi^2$, whose [kernel of an isogeny](../../../../../../kernel-of-an-isogeny.md) is exactly $E(\mathbb F_{p^2})$. Multiplicativity of degree gives the same product.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
