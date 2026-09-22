<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The map $F$ is a [nonsingular transformation](../../../../../../../nonsingular-transformation.md) with respect to $\omega$ when

$$
\omega(N)=0\quad\Longrightarrow\quad
\omega(F^{-1}(N))=0.
$$

Equivalently, the [pushforward measure](../../../../../../../pushforward-measure.md) $F_*\omega(B)=\omega(F^{-1}(B))$ satisfies $F_*\omega\ll\omega$.

For an essentially bounded observable $g$, define the [Koopman operator](../../../../../../../koopman-operator.md)

$$
\boxed{K_Fg=g\circ F.}
$$

Nonsingularity makes this well defined on almost-everywhere equivalence classes. By the [Radon-Nikodym theorem](../../../../../../../radon-nikodym-theorem.md),

$$
\|K_Fg\|_2^2
=\int|g|^2\,d(F_*\omega)
=\int|g|^2\frac{d(F_*\omega)}{d\omega}\,d\omega.
$$

Consequently the [bounded Koopman operator criterion](../../../../../../../bounded-koopman-operator-criterion.md) is

$$
\boxed{
K_F:L^2(\omega)\to L^2(\omega)\text{ is bounded}
\iff
\frac{d(F_*\omega)}{d\omega}\in L^\infty(\omega).}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 358](../../../../paper-358-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
