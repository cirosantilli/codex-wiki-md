<h1 id="12g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $r=\|X\|<1$. By [submultiplicativity of the operator norm](../../../../../../submultiplicativity-of-the-operator-norm.md), $\|X^k\|\le r^k$, so the [Neumann series](../../../../../../neumann-series.md) converges absolutely in the complete finite-dimensional matrix space. Its partial sums satisfy

$$
(I-X)\sum_{k=0}^N X^k=\left(\sum_{k=0}^N X^k\right)(I-X)=I-X^{N+1}.
$$

Taking limits gives **the inverse and a quantitative remainder bound**:

$$
\boxed{f(X)=\sum_{k=0}^{\infty}X^k,\qquad
\left\|f(X)-\sum_{k=0}^N X^k\right\|\le\frac{r^{N+1}}{1-r}.}
$$

To establish two actual [Fréchet derivatives](../../../../../../frechet-derivative.md), use the [resolvent identity](../../../../../../resolvent-identity.md)

$$
f(X+H)-f(X)=f(X+H)Hf(X).
$$

For fixed $X\in U$ and sufficiently small $H$, factor $I-X-H=(I-X)(I-f(X)H)$ and apply the [Neumann series](../../../../../../neumann-series.md) to the second factor. This proves that $X+H\in U$, that $f(X+H)$ is locally bounded, and that $f(X+H)-f(X)=O(\|H\|)$. Subtracting $f(X)Hf(X)$ in the identity leaves $O(\|H\|^2)$. Thus $Df(X)[H]=f(X)Hf(X)$ is the [Fréchet derivative](../../../../../../frechet-derivative.md).

Near zero, $f(X)=I+X+O(\|X\|^2)$, uniformly in the [operator norm](../../../../../../operator-norm.md). Hence, as a linear operator in $H$,

$$
Df(X)[H]=H+XH+HX+O(\|X\|^2\|H\|).
$$

This proves differentiability of $Df$ at zero, giving

$$
\boxed{Df(0)[H]=H,\qquad D^2f(0)[H,K]=HK+KH.}
$$

The order of multiplication matters: the second [Fréchet derivative](../../../../../../frechet-derivative.md) is the symmetric [bilinear map](../../../../../../bilinear-map.md) $HK+KH$, not $2HK$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12G](../../12g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
