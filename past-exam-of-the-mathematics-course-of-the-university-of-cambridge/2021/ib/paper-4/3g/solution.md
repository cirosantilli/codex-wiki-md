<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

The hypothesis says that $f$ has a zero of [order](../../../../../order-of-a-zero-of-a-holomorphic-function.md) $k$ at $a$, so write

$$
f(z)=(z-a)^kg(z),
\qquad
g(a)\ne0,
$$

with $g$ holomorphic near $a$. Differentiating gives

$$
f'(z)=(z-a)^{k-1}\bigl(kg(z)+(z-a)g'(z)\bigr).
$$

Choose $\delta>0$ so small that the closed disc $\overline D(a,\delta)$ lies in the domain, $g$ never vanishes there, and the parenthesized factor never vanishes there. Thus $a$ is the only critical point of $f$ in that disc.

On the boundary circle, $f$ is nonzero. Set

$$
\varepsilon=\min_{|z-a|=\delta}|f(z)|>0.
$$

If $0<|b|<\varepsilon$, then $|b|<|f(z)|$ on the boundary. [Rouché's theorem](../../../../../rouche-s-theorem.md) applied to $f$ and $f-b$ says that $f-b$ has the same number of zeros in $D(a,\delta)$ as $f$, namely $k$, counted with multiplicity.

None of these zeros is $a$ because $b\ne0$, and none is a critical point because $f'$ has no other zero in the disc. Every zero of $f-b$ is therefore simple. Hence there are exactly

$$
\boxed{k\text{ distinct }z\in D(a,\delta)\text{ with }f(z)=b}.
$$

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
