<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $x:S\to G$, define

$$
T_x:G\times_kS\to G,
\qquad(g,s)\mapsto x(s)g.
$$

Then $T_{x/S}=(T_x,\operatorname{pr}_2)$ is an $S$-morphism, and translation by $x^{-1}$ is its inverse.

Because an isomorphism preserves relative differentials and $T_{x/S}$ lies over $S$,

$$
T_{x/S}^*\Omega_{G\times S/S}\cong\Omega_{G\times S/S}.
$$

Using base change, $\Omega_{G\times S/S}\cong\operatorname{pr}_1^*\Omega_{G/k}$, while the left side is $T_x^*\Omega_{G/k}$. Pulling this isomorphism back along the identity section $e\times1_S$ gives

$$
x^*\Omega_{G/k}\cong\mathcal O_S\otimes_k\Omega_{G/k}(e).
$$

Finally take $S=G$ and $x=1_G$. This yields the [invariant differential on a group scheme](../../../../../../invariant-differential-on-a-group-scheme.md) trivialization

$$
\Omega_{G/k}\cong\mathcal O_G\otimes_k\Omega_{G/k}(e),
$$

so $\Omega_{G/k}$ is a free $\mathcal O_G$-module.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
