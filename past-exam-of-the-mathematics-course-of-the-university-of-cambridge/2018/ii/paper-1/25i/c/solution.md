<h1 id="25i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose first that $\overline{f(X)}=Y$. If $g\in\ker f^*$, then $g\circ f=0$, so the zero set of the regular function $g$ contains $f(X)$ and hence its closure $Y$. Thus $g=0$ in the [coordinate ring](../../../../../../coordinate-ring.md) $k[Y]$, and $f^*$ is injective.

Conversely, if $\overline{f(X)}$ were a proper closed subset of $Y$, its vanishing ideal in $k[Y]$ would contain a nonzero regular function $g$. Then $g$ vanishes on $f(X)$, so $f^*(g)=0$, contradicting injectivity. Therefore

$$
\boxed{\ \overline{f(X)}=Y\iff f^*:k[Y]\to k[X]\text{ is injective}.\ }
$$

This is the coordinate-ring criterion for a [dominant morphism of affine varieties](../../../../../../dominant-morphism-of-affine-varieties.md).

For an irreducible affine variety, define dimension by

$$
\dim X=\operatorname{trdeg}_k k(X),
\qquad k(X)=\operatorname{Frac}(k[X]).
$$

Irreducibility makes both coordinate rings [integral domains](../../../../../../integral-domain.md). The injective map $f^*:k[Y]\hookrightarrow k[X]$ extends to an embedding of function fields

$$
k(Y)\hookrightarrow k(X).
$$

An algebraically independent family in $k(Y)$ remains algebraically independent in $k(X)$, so the [dimension of an irreducible affine variety by transcendence degree](../../../../../../dimension-of-an-irreducible-affine-variety-by-transcendence-degree.md) gives

$$
\boxed{\ \dim X\geq\dim Y.\ }
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [25I](../../25i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
