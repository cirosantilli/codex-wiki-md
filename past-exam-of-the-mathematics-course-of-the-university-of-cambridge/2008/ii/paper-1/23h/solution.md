<h1 id="23h/solution">Solution</h1>

↑ **Parent:** [23H](../23h.md)

A [Riemann surface](../../../../../riemann-surfaces.md) is a connected one-complex-dimensional manifold with [holomorphic](../../../../../complex-differentiability-at-a-point.md) chart transitions. A map between such surfaces is [holomorphic](../../../../../complex-differentiability-at-a-point.md) when all its local coordinate expressions are [holomorphic](../../../../../complex-differentiability-at-a-point.md); it is [biholomorphic](../../../../../biholomorphism.md) when it is a bijection whose inverse is also [holomorphic](../../../../../complex-differentiability-at-a-point.md).

The open mapping theorem says a nonconstant [holomorphic](../../../../../complex-differentiability-at-a-point.md) function on a connected complex domain maps open sets to open sets. Applied in charts, with the [identity theorem](../../../../../identity-theorem.md) excluding a locally constant portion, it makes a nonconstant [holomorphic map](../../../../../holomorphic-map.md) of connected surfaces open. If the domain is compact, its image is compact and hence closed in the Hausdorff target. A nonempty set both open and closed in a connected target is the whole target. Therefore the map is surjective, without any appeal to degree.

For a biholomorphism $\phi:\Delta^*\to\Delta^*$, both $\phi$ and its inverse are bounded near the missing origin. They extend holomorphically across zero by removability: in a [Laurent series](../../../../../laurent-series.md) a negative coefficient satisfies $|a_{-m}|\leq M r^m$ on radius $r$, hence vanishes as $r\to0$. Let the extensions be $F,G$. Their images lie in $\Delta$: a modulus-one interior value would force a bounded [holomorphic map](../../../../../holomorphic-map.md) to be constant by the [maximum modulus principle](../../../../../maximum-modulus-principle.md). The compositions $GF$ and $FG$ equal the identity on the punctured disk and thus on the disk by [continuity](../../../../../continuous-function.md). If $F(0)\ne0$, then $G(F(0))$ would be nonzero because the original inverse maps $\Delta^*$ into itself, contradicting $G(F(0))=0$. Consequently

$$
\boxed{F:\Delta\to\Delta\text{ is biholomorphic and }F(0)=0.}
$$

For the final assertion only [continuity](../../../../../continuous-function.md) on $R$ and holomorphicity on $R\setminus\{p\}$ are needed; the printed stronger description is redundant. Choose a target chart about $f(p)$ and, by [continuity](../../../../../continuous-function.md), a small source chart mapped into it. The resulting scalar function is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on a punctured disk and bounded near its center, so the same Laurent argument removes its singularity. [continuity](../../../../../continuous-function.md) makes the extension's central value equal the prescribed value. Thus $f$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) also at $p$.

## ↑ Ancestors (10)

1. [23H](../23h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
