<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Ward identity](../../../../ward-identity.md) implies $q^\mu\Pi_{\mu\nu}=0$. [Lorentz invariance](../../../../lorentz-invariance.md) then gives $\Pi_{\mu\nu}=(q^2g_{\mu\nu}-q_\mu q_\nu)\Pi$, so $g^{\mu\nu}\Pi_{\mu\nu}=(d-1)q^2\Pi$. The [gamma matrices](../../../../gamma-matrices.md) satisfy $\gamma_\mu\not k\gamma^\mu=(2-d)\not k$. Odd [traces](../../../../matrix-trace.md) vanish, and therefore

$$
g^{\mu\nu}\operatorname{tr}[\gamma_\mu(\not k+m)\gamma_\nu(\not k+\not q+m)]
=4[-(d-2)k\cdot(k+q)+dm^2].
$$

Substituting gives the requested [scalar](../../../../scalar.md) coefficient:

$$
\boxed{\Pi(q^2)=\frac{4ie^2}{(d-1)q^2}\int_k
\frac{-(d-2)k\cdot(k+q)+dm^2}{[(k+q)^2-m^2+i0][k^2-m^2+i0]}.}
$$

To extract the [ultraviolet divergence](../../../../ultraviolet-divergence.md) without introducing a [Feynman parameter](../../../../feynman-parameter.md), set $A=(k+q)^2-m^2$, $B=k^2-m^2$ and use

$$
2k\cdot(k+q)=A+B+2m^2-q^2.
$$

Translation invariance of [dimensional regularization](../../../../dimensional-regularization.md) gives $\int_kA^{-1}=\int_kB^{-1}=\mathcal I_1$. Consequently

$$
\Pi(q^2)=\frac{4ie^2}{(d-1)q^2}\left[-(d-2)\mathcal I_1+
\left(2m^2+\frac{d-2}{2}q^2\right)\mathcal I_2(q^2)\right].
$$

In the [pole](../../../../pole.md) coefficient one may set $d=4$: the bracket becomes

$$
\frac{i}{16\pi^2\epsilon}[-2m^2+2m^2+q^2]
=\frac{iq^2}{16\pi^2\epsilon}.
$$

Thus the [ultraviolet pole of QED vacuum polarization](../../../../ultraviolet-pole-of-qed-vacuum-polarization.md) is

$$
\boxed{\Pi(q^2)\big|_{\rm UV}=-\frac{e^2}{12\pi^2\epsilon},\qquad
\Pi_{\mu\nu}\big|_{\rm UV}=-\frac{e^2}{12\pi^2\epsilon}(q^2g_{\mu\nu}-q_\mu q_\nu).}
$$

The cancellation of the apparent $m^2/q^2$ divergence is essential: [gauge invariance](../../../../gauge-invariance.md) forbids a [photon](../../../../photon.md) [mass](../../../../mass.md) [counterterm](../../../../counterterm.md). The scalar result at $q^2=0$ is understood by continuation after this cancellation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
