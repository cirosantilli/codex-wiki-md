<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

[Lorentz-covariant](../../../../lorentz-covariance.md) [tensor integration](../../../../lorentz-covariant-rank-two-loop-reduction.md) replaces $q_\mu q_\nu$ by $g_{\mu\nu}q^2/d$. The numerator consequently contributes $(d-1)k^2q^2/d$. The supplied master integral with powers $a=1,b=3$ gives

$$
\int\frac{d^dq}{(2\pi)^d}\frac{q^2}{(q^2+D)^3}
=\frac{i}{(4\pi)^{d/2}}\frac d4\Gamma(\epsilon/2)D^{-\epsilon/2}.
$$

Inserting the corrected parameter integral gives

$$
i\Pi_{\mathrm{ex}}=\frac{2i(d-1)e^2\mu^\epsilon k^2}{(4\pi)^{d/2}}\Gamma(\epsilon/2)\int_0^1(1-x)D^{-\epsilon/2}dx.
$$

The pole uses $\Gamma(\epsilon/2)=2/\epsilon+O(1)$, $D^{-\epsilon/2}=1+O(\epsilon)$ and $\int_0^1(1-x)dx=1/2$. Thus

$$
\boxed{i\Pi_{\mathrm{loop,div}}=i\frac{3e^2}{8\pi^2\epsilon}k^2.}
$$

There is no momentum-independent pole at $\lambda=0$ in this transverse gauge after removing the [photon tadpole](../../../../tadpole-diagram.md). The [two-point](../../../../two-point-correlation-function.md) [counterterm](../../../../counterterm.md) insertion is $-i(\delta Z_\phi k^2+\delta M^2)$, so [minimal subtraction](../../../../minimal-subtraction-scheme.md) requires

$$
\boxed{\delta Z_\phi=\frac{3e^2}{8\pi^2\epsilon},\qquad \delta M^2=0\qquad(d=4-\epsilon).}
$$

These coefficients cancel the actual [one-loop](../../../../loop-feynman-diagram.md) insertion derived from the [action](../../../../action.md). Applying the misprinted weight in part e would give a wave-function pole four times too small. In a $d=4-2\varepsilon$ convention the same answer is $\delta Z_\phi=3e^2/(16\pi^2\varepsilon)$. Finally, $\delta M^2=0$ does not mean that the bare [mass parameter](../../../../mass.md) is unchanged: $Z_\phi m_0^2=m^2$ gives $m_0^2-m^2=-m^2\delta Z_\phi+O(e^4)$. [Photon](../../../../photon.md), charge and [quartic](../../../../quartic-interaction.md) [counterterms](../../../../counterterm.md) require their respective [Green functions](../../../../green-s-function-split.md) and cannot be determined from this [scalar](../../../../scalar-field.md) [two-point function](../../../../two-point-correlation-function.md) alone.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
