<h1 id="section-b/b6/transversality-and-tensor-conventions">Transversality and tensor conventions</h1>

↑ **Parent:** [Solution](solution.md)

Write a nonzero [vacuum](../../../../vacuum.md) [plane electromagnetic wave](../../../../plane-electromagnetic-wave.md) with [wavevector](../../../../wavevector.md) $\mathbf k=(\omega/c)\mathbf s$, where $\mathbf s$ is a unit propagation direction. Its propagation [Lorentz four-vector](../../../../four-vector.md) is $K^\mu=(\omega/c,\mathbf k)$, or, up to a scalar normalization in any one frame, $n^\mu=(1,\mathbf s)$. It is null because $K_\mu K^\mu=0$.

Choose coordinates $x^\mu=(ct,\mathbf x)$ and [Minkowski metric](../../../../minkowski-metric.md) $\eta_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$. With the supplied three-dimensional boost formulas, a consistent convention assigns the printed array to upper-index components,

$$
F^{0i}=-E_i/c,\qquad F^{ij}=-\epsilon_{ijk}B_k.
$$

The [index conventions for the electromagnetic field tensor](../../../../index-conventions-for-the-electromagnetic-field-tensor.md) then require $F_{0i}=+E_i/c$ and $F_{ij}=F^{ij}$ when both indices are lowered. The printed lower-index label therefore cannot be kept together with its electric signs and a forward propagation vector in this convention.

This is not merely an arbitrary overall sign. For a valid forward wave with $\mathbf s=\widehat{\mathbf z}$, $\mathbf E=E_0\widehat{\mathbf x}$ and $\mathbf B=(E_0/c)\widehat{\mathbf y}$, multiplying the printed array, unchanged, by $n^\mu=(1,0,0,1)$ gives an $x$ component $-2E_0/c$, rather than zero. One consistent repair is to retain the printed array as $F^{\mu\nu}$ and contract with $n_\mu=(1,-\mathbf s)$. Equivalently, lower both tensor indices before forming the contraction asked for in the question.

Using that corrected lower-index tensor gives

$$
n^\mu F_{\mu\nu}
=\left(-\frac{\mathbf s\cdot\mathbf E}{c},\frac{\mathbf E}{c}+\mathbf s\times\mathbf B\right).
$$

To establish both electric and magnetic transversality, include the [dual electromagnetic field tensor](../../../../dual-electromagnetic-field-tensor.md). Choose $\widetilde F^{0i}=-B_i$ and $\widetilde F^{ij}=\epsilon_{ijk}E_k/c$; lowering both indices then gives

$$
n^\mu\widetilde F_{\mu\nu}
=\left(-\mathbf s\cdot\mathbf B,\mathbf B-\frac{\mathbf s\times\mathbf E}{c}\right).
$$

The source-free plane-wave [Maxwell equations](../../../../maxwell-equations-split.md) are precisely the pair of covariant conditions

$$
\boxed{n^\mu F_{\mu\nu}=0,\qquad n^\mu\widetilde F_{\mu\nu}=0.}
$$

Their temporal components give $\mathbf k\cdot\mathbf E=0$ and $\mathbf k\cdot\mathbf B=0$. Their spatial components give the associated amplitude and orientation relations, $\mathbf E/c=-\mathbf s\times\mathbf B$ and $\mathbf B=\mathbf s\times\mathbf E/c$.

To see the [Lorentz covariance](../../../../lorentz-covariance.md) explicitly, let $V_\nu=K^\mu F_{\mu\nu}$. It is a [covector](../../../../covector.md), so if $V_\nu=0$ in one [inertial frame](../../../../inertial-frame.md), its [Lorentz transformation](../../../../lorentz-transformation.md) is also zero in every other [inertial frame](../../../../inertial-frame.md). The same is true of $K^\mu\widetilde F_{\mu\nu}$. Since the transformed wave still has $K'^0>0$ and $|\mathbf k'|=\omega'/c$, their temporal components imply

$$
\boxed{\mathbf k'\cdot\mathbf E'=\mathbf k'\cdot\mathbf B'=0.}
$$

Here $K^\mu$, rather than a vector renormalized to have temporal component one in every frame, is the actual [Lorentz four-vector](../../../../four-vector.md); multiplying a zero contraction by a nonzero normalization does not affect the argument.

Finally, the two scalar perpendicularity statements alone are not equivalent to one tensor contraction. They do not enforce the amplitude relation between $\mathbf E$ and $\mathbf B$. Conversely $n^\mu F_{\mu\nu}=0$ alone cannot exclude a longitudinal [magnetic field](../../../../magnetic-field-split.md): adding $B_\parallel\mathbf s$ leaves its cross product unchanged. For a genuine source-free [plane electromagnetic wave](../../../../plane-electromagnetic-wave.md), the remaining [Maxwell equations](../../../../maxwell-equations-split.md) supply that missing constraint, and both tensor contractions vanish. This qualification and the corrected index placement are necessary for the intended invariance argument.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [B6](../b6.md)
3. [Section B](../../section-b.md)
4. [2019](../../../2019-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
