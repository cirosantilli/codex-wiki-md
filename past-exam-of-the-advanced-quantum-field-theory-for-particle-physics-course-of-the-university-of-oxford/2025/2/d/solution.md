<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the right panel of part [a](../a.md), $p$ enters the [fermion](../../../../fermion.md) line, $p'=p+q$ leaves it, and a virtual [photon](../../../../photon.md) of [momentum](../../../../momentum-split.md) $k$ bridges the external [photon](../../../../photon.md) vertex. Write $\Gamma^\mu=\gamma^\mu+\Lambda^\mu$ and $F_1=1+F_1^{(1)}+\cdots$. The one-loop [amplitude](../../../../wave-amplitude.md) is

$$
\begin{aligned}
-ie\Lambda^\mu={}&\int_k(-ie\gamma^\alpha)
\frac{i(\not p'-\not k+m)}{(p'-k)^2-m^2+i0}
(-ie\gamma^\mu)\frac{i(\not p-\not k+m)}{(p-k)^2-m^2+i0}
(-ie\gamma^\beta)\frac{-ig_{\alpha\beta}}{k^2+i0},\\
&\boxed{\Lambda^\mu=-ie^2\int_k
\frac{\gamma^\alpha(\not p'-\not k+m)\gamma^\mu(\not p-\not k+m)\gamma_\alpha}
{[k^2+i0][(p'-k)^2-m^2+i0][(p-k)^2-m^2+i0]}.}
\end{aligned}
$$

This [Feynman integral](../../../../feynman-integral.md) has a logarithmic [superficial degree of divergence](../../../../superficial-degree-of-divergence.md). Its [ultraviolet pole](../../../../ultraviolet-pole.md) is independent of the external [momenta](../../../../momentum-split.md) and $m$, because every such numerator insertion or denominator correction lowers the large-$k$ degree. Preserve an auxiliary positive [mass](../../../../mass.md) $M$ while extracting the [ultraviolet pole](../../../../ultraviolet-pole.md); setting everything to zero would create a [scaleless integral](../../../../scaleless-integral.md) and conceal the cancellation of [ultraviolet](../../../../ultraviolet.md) and [infrared divergences](../../../../infrared-divergence.md).

The leading numerator is $\gamma^\alpha\not k\gamma^\mu\not k\gamma_\alpha$. Symmetric integration replaces $k_\rho k_\sigma$ by $g_{\rho\sigma}k^2/d$. Two contractions of [gamma matrices](../../../../gamma-matrices.md) then give

$$
\gamma^\alpha\not k\gamma^\mu\not k\gamma_\alpha
\ \longmapsto\ \frac{(d-2)^2}{d}k^2\gamma^\mu,
\qquad
\operatorname{tr}\left[\gamma^\alpha\not k\gamma^\mu\not k\gamma_\alpha\gamma_\mu\right]
=4(d-2)^2k^2.
$$

For the [auxiliary-mass extraction of ultraviolet poles](../../../../auxiliary-mass-extraction-of-ultraviolet-poles.md),

$$
J_M=\int_k\frac{k^2}{(k^2-M^2+i0)^3}
=\int_k\left[\frac1{(k^2-M^2+i0)^2}+\frac{M^2}{(k^2-M^2+i0)^3}\right],
\qquad J_M\big|_{\rm UV}=\frac{i}{16\pi^2\epsilon}.
$$

The second term is [ultraviolet](../../../../ultraviolet.md) convergent. Thus

$$
\frac1{4d}\operatorname{tr}(\Lambda^\mu\gamma_\mu)\big|_{\rm UV}
=-ie^2\frac{(d-2)^2}{d}J_M\big|_{\rm UV},
\qquad
\boxed{F_1^{(1)}(q^2)\big|_{\rm UV}=\frac{e^2}{16\pi^2\epsilon}.}
$$

The [ultraviolet pole of the QED vertex](../../../../ultraviolet-pole-of-the-qed-vertex.md) is therefore $\Lambda^\mu|_{\rm UV}=e^2\gamma^\mu/(16\pi^2\epsilon)$. The Pauli structure has zero [trace](../../../../matrix-trace.md) against $\gamma_\mu$ and no [ultraviolet pole](../../../../ultraviolet-pole.md) at this order.

**Form-factor qualification.** The two [electron electromagnetic vertex form factors](../../../../electron-electromagnetic-vertex-form-factors.md) in the source describe matrix elements between external [on shell](../../../../on-shell.md) [Dirac spinors](../../../../dirac-spinor.md). A general [off shell](../../../../off-shell.md) vertex has more structures, so the unprojected [trace](../../../../matrix-trace.md) is not a projector for the complete finite on-shell $F_1$. It does correctly isolate the divergent local $\gamma^\mu$ coefficient, which is all that is required here.

## ↑ Ancestors (12)

1. [D](../d.md)
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
