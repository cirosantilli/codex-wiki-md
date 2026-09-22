<h1 id="31a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\dot z=F(z)$ be a $C^1$ planar system on a simply connected domain $D$. The [Bendixson-Dulac criterion](../../../../../../bendixson-dulac-theorem.md) states that if some $B\in C^1(D)$ makes

$$
\nabla\mathbin{\cdot}(BF)
$$

have one sign throughout $D$ and not vanish identically on any open subset, then $D$ contains no periodic orbit.

Indeed, if a periodic orbit $\Gamma$ bounded a region $\Omega\subset D$, then $F$ and hence $BF$ would be tangent to $\Gamma$. Its normal flux would therefore vanish. The divergence theorem would give

$$
0=\int_\Gamma BF\mathbin{\cdot}n\,ds
=\iint_\Omega\nabla\mathbin{\cdot}(BF)\,dA,
$$

contradicting the sign hypothesis. Taking $B=1$ gives the usual Bendixson divergence criterion.

The stability version of the divergence test concerns an existing periodic orbit $\gamma$ of period $T$. Liouville's formula for the variational equation shows that its nontrivial [Floquet multiplier](../../../../../../floquet-multiplier.md) is

$$
\rho=\exp\left(
\int_0^T\nabla\mathbin{\cdot}F(\gamma(t))\,dt
\right).
$$

**Thus the [divergence test for a planar periodic orbit](../../../../../../divergence-test-for-a-planar-periodic-orbit.md) says that $\gamma$ is asymptotically stable if the integral is negative and unstable if it is positive.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31A](../../31a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
