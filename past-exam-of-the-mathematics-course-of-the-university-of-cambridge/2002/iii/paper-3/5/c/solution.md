<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $d=2n$ with $n\geq2$, and let $E$ be the [splitting field](../../../../../../splitting-field.md). The root set of $X^{q^{2n}}+X^{q^2}+tX$ is an $n$-dimensional [vector space](../../../../../../vector-space-split.md) over $\mathbb F_{q^2}$, by the argument of part (a) with $q$ replaced by $q^2$.

The constants $\mathbb F_{q^2}$ really occur inside $E$, rather than only in the ambient [algebraic closure](../../../../../../algebraic-closure.md). Choose a nonzero root $\alpha$. For every $c\in\mathbb F_{q^2}$, $c\alpha$ is also a root, so both elements lie in $E$ and

$$
c=\frac{c\alpha}{\alpha}\in E.
$$

Let $K=\mathbb F_{q^2}(t)$. Since $K/\mathbb F_q(t)$ is Galois of degree two,

$$
H=\operatorname{Gal}(E/K)\triangleleft G,
\qquad\boxed{[G:H]=2.}
$$

This index statement does not require proving that $E$ has no still larger constant [field](../../../../../../field.md).

As an extension of $K$, $E$ is the [splitting field](../../../../../../splitting-field.md) of the same [polynomial](../../../../../../polynomial-split.md). Applying part (b) with base constant size $q^2$ and dimension $n$ gives

$$
SL(n,q^2)\leq H\leq GL(n,q^2).
$$

The [special linear group](../../../../../../special-linear-group.md) is the kernel of determinant in the [general linear group](../../../../../../general-linear-group.md), so every element of $H$ normalizes it. Therefore **$H$ is the required normal index-two subgroup normalizing $SL(d/2,q^2)$**.

In fact the full group is semilinear over $\mathbb F_{q^2}$: an element outside $H$ acts on constants as $c\mapsto c^q$ and satisfies $g(cv)=c^qg(v)$. [Field](../../../../../../field.md) automorphisms preserve determinant one, so this also explains the [normalizer](../../../../../../normalizer.md) behavior geometrically. This is the [quadratic constant extension of a q-squared linearized splitting field](../../../../../../quadratic-constant-extension-of-a-q-squared-linearized-splitting-field.md), not the [polynomial](../../../../../../polynomial-split.md) of part (b) with its $X^q$ term unchanged.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
