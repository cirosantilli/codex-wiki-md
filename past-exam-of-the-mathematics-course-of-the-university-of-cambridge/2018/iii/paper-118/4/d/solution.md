<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the usual connected-manifold convention for this assertion. Suppose, for contradiction, that $H^2(M,\mathcal O_M)=0$. The [Dolbeault theorem](../../../../../../dolbeault-theorem.md) gives $H^{0,2}=0$, and the [Hodge decomposition theorem for compact Kähler manifolds](../../../../../../hodge-decomposition-theorem-for-compact-kahler-manifolds.md) and its conjugation symmetry give $H^{2,0}=0$. Hence every real class in $H^2(M,\mathbb R)$ has a real [harmonic differential form](../../../../../../harmonic-differential-form.md) of type $(1,1)$ as its representative.

The [intersection form](../../../../../../intersection-form.md) is $Q([u],[v])=\int_Mu\wedge v$. Its value on the Kähler class is positive: $Q([\omega],[\omega])=\int_M\omega^2>0$. Every real harmonic $(1,1)$ form splits uniquely as $c\omega+u_0$, with $u_0$ primitive and $c$ constant. Indeed, $\Lambda u$ is a [harmonic function](../../../../../../harmonic-function.md), hence constant by [connectedness](../../../../../../connected-space.md), and $\Lambda\omega=2$; subtracting $c\omega$ kills $\Lambda u$, and part (b) makes $u_0$ primitive.

Part (c) gives $*u_0=-u_0$, while $\omega\wedge u_0=0$. Thus

$$
Q([\omega],[u_0])=0,\qquad Q([u_0],[u_0])=-\|u_0\|_{L^2}^2<0\quad(u_0\ne0).
$$

This proves the [Hodge index theorem for compact Kähler surfaces](../../../../../../hodge-index-theorem-for-compact-kahler-surfaces.md) in this case: $Q$ has [signature](../../../../../../signature-of-a-quadratic-form.md) $(1,b_2-1)$.

On the alleged two-dimensional [totally isotropic subspace](../../../../../../totally-isotropic-subspace.md) $V$, the [linear functional](../../../../../../linear-functional.md) $v\mapsto Q(v,[\omega])$ has a nonzero vector in its [kernel](../../../../../../kernel-of-a-linear-map.md). Its [harmonic differential form](../../../../../../harmonic-differential-form.md) representative is primitive, so the preceding negative-definiteness statement gives $Q(v,v)<0$, contradicting the vanishing of $Q$ on $V$. Therefore

$$
\boxed{\dim_{\mathbb R}V=2,\quad Q|_{V\otimes V}=0\ \Longrightarrow\ H^2(M,\mathcal O_M)\ne0.}
$$

[Connectedness](../../../../../../connected-space.md) is essential if one's definition of a manifold allows disconnected spaces. For $M=Y\sqcup Y$, with $Y=\mathbb{CP}^1\times\mathbb{CP}^1$, one has $H^2(M,\mathcal O_M)=0$. Take on each component the pullback of the degree-two class from its first factor. Each class has square zero, and their mutual pairing is zero because their supports lie on different components. Their span is then a two-dimensional [totally isotropic subspace](../../../../../../totally-isotropic-subspace.md), disproving the unqualified disconnected version.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
