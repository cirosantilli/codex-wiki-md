<h1 id="25i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No.** The missing point is not assumed to complete $S$ as a smooth surface, so the hypotheses of the global [Gauss-Bonnet theorem](../../../../../../gauss-bonnet-theorem.md) do not apply to $S\cup\{p\}$.

For a concrete counterexample, rotate a smooth simple arc $(r(s),z(s))$, parametrized by arc length for $0\leq s<L$, about the $z$-axis. Arrange that it starts smoothly on the axis,

$$
r(0)=0,\qquad r'(0)=1,
$$

stays in $r>0$ for $0<s<L$, and converges to another point of the axis as $s\uparrow L$, with

$$
r'(s)\longrightarrow-a,\qquad0\leq a<1.
$$

The endpoint is omitted. The resulting [surface of revolution](../../../../../../surface-of-revolution.md) is diffeomorphic to $\mathbb S^2$ minus one point, and adjoining its limiting endpoint makes the set compact.

For an arc-length surface of revolution,

$$
K=-\frac{r''}{r},
\qquad
dA=r\,ds\,d\theta.
$$

Therefore the [total Gaussian curvature of a punctured surface with a singular compactification point](../../../../../../total-gaussian-curvature-of-a-punctured-surface-with-a-singular-compactification-point.md) is

$$
\int_SK\,dA
=-2\pi\int_0^Lr''(s)\,ds
=2\pi(1+a),
$$

which can take values different from $4\pi$. Compactness of the one-point closure alone therefore does not determine the integral.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
