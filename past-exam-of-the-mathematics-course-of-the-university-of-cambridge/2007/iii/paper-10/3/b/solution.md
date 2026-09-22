<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\widetilde W$ be the given regular irreducible family. Write $a=(x,y)$ and $a\wedge b=x_1y_2-y_1x_2$. Define the strongly integrated operator

$$
P=\frac1\pi\int_{\mathbb R^2}e^{-|a|^2/2}\widetilde W(a)\,da.
$$

The Gaussian is integrable and the operators are unitary, so the integral defines a [bounded operator](../../../../../../continuous-linear-operator.md) on each [vector](../../../../../../vector.md). The Weyl relation and $\widetilde W(a)^*=\widetilde W(-a)$ give $P^*=P$. For its square, the coefficient at $\widetilde W(c)$ is

$$
\frac1{\pi^2}\int e^{-(|a|^2+|c-a|^2)/2}e^{ia\wedge c}da
=\frac1\pi e^{-|c|^2/2},
$$

by the two-dimensional [Gaussian integral](../../../../../../gaussian-integral.md). Thus $P^2=P$. The same Gaussian integration, with an inserted Weyl operator, gives

$$
\boxed{P\widetilde W(b)P=e^{-|b|^2/2}P.}
$$

This is the [Gaussian projection in a Weyl representation](../../../../../../gaussian-projection-in-a-weyl-representation.md).

It is nonzero. Otherwise all its conjugates would vanish; the Weyl relation makes their [matrix](../../../../../../matrix.md) coefficients the Fourier transforms of $e^{-|a|^2/2}(\widetilde W(a)\xi,\eta)$, with the dual variable $2b\wedge a$. Uniqueness of the [Fourier transform](../../../../../../fourier-transform.md) of an integrable function would make each such function zero. [Strong continuity](../../../../../../strong-continuity.md) then makes its value at zero vanish, contradicting $(\xi,\xi)>0$ for a nonzero [vector](../../../../../../vector.md).

Choose a unit [vector](../../../../../../vector.md) $v\in PH$. Irreducibility makes the span of $\widetilde W(a)v$ dense. If $w\in PH$ is perpendicular to $v$, the boxed identity makes it perpendicular to this entire span, so $w=0$. Hence $P$ has [rank](../../../../../../rank-one-quadratic-form.md) one, and its identity gives $(\widetilde W(a)v,v)=e^{-|a|^2/2}$.

In the concrete representation of part (a), the Gaussian $v_0(t)=(2/\pi)^{1/4}e^{-t^2}$ has precisely this expectation. With the linear-in-first inner-product convention, both orbit families have [Gram matrix](../../../../../../gram-matrix.md)

$$
(\widetilde W(a)v,\widetilde W(b)v)=e^{ia\wedge b}e^{-|a-b|^2/2}
=(W(a)v_0,W(b)v_0).
$$

Therefore the map $\sum c_jW(a_j)v_0\mapsto\sum c_j\widetilde W(a_j)v$ is well-defined and isometric. Its source and target spans are dense, so it extends to a [unitary operator](../../../../../../unitary-operator.md) intertwiner. This proves the **[unitary equivalence](../../../../../../unitary-equivalence.md)**, the [Stone-von Neumann theorem](../../../../../../stone-von-neumann-theorem.md) in the normalization of this question, rather than invoking that theorem as the proof.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
