<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $m_A=ef$, $r=1+h/f$, and $H=\partial\cdot A-\xi m_A r^2\pi$, so the given $G=H/\sqrt\xi$ contributes $\mathcal L_{\rm gf}=-H^2/(2\xi)$. Its quadratic cross term is $+m_A\pi\partial\cdot A$, which cancels $m_AA\cdot\partial\pi$ from the scalar kinetic term after [integration by parts](../../../../integration-by-parts.md). The free vector and would-be [Goldstone boson](../../../../goldstone-boson.md) [propagators](../../../../propagator.md) are therefore diagonal; $\pi$ has gauge-dependent [mass](../../../../mass.md) squared $\xi m_A^2$.

The field-dependent factor $r^2$ cancels more than just the constant-coefficient mixing, but a residual derivative interaction remains. Indeed,

$$
\begin{aligned}
\mathcal L_{\rm mix}+\mathcal L_{\rm gf,cross}
&=m_A r^2(A\cdot\partial\pi+\pi\partial\cdot A)\\
&=\partial_\mu(m_A r^2A^\mu\pi)-m_A\pi A^\mu\partial_\mu r^2\\
&\simeq-2e\left(1+\frac hf\right)\pi A^\mu\partial_\mu h.
\end{aligned}
$$

Thus the [nonlinear R-xi gauge in polar Higgs variables](../../../../nonlinear-r-xi-gauge-in-polar-higgs-variables.md) removes quadratic mixing; it does not remove every interaction containing $A$ and $\pi$.

Use the [gauge transformation](../../../../gauge-transformation.md) in part [b](../b.md). Since $h$ is invariant,

$$
\delta_\alpha H=-\frac1e\Box\alpha-\xi m_A r^2f\alpha
=-\frac1e[\Box+\xi m_A^2r^2]\alpha.
$$

The factor $-1/(e\sqrt\xi)$ in $\delta G/\delta\alpha$ is field independent and is absorbed into the [partition function](../../../../canonical-partition-function.md) normalization. Exponentiating the remaining [Faddeev-Popov determinant](../../../../faddeev-popov-determinant.md) with the sign convention of part [a](../a.md) gives

$$
\boxed{\mathcal L_{\rm gh}=-\bar c\left[\Box+\xi e^2(f+h)^2\right]c
=-\bar c(\Box+\xi m_A^2)c
-2\xi e^2fh\bar cc-\xi e^2h^2\bar cc.}
$$

The [ghost coupling in the Abelian Higgs model](../../../../ghost-coupling-in-the-abelian-higgs-model.md) therefore survives even though the [gauge group](../../../../gauge-group.md) is Abelian: these [Faddeev-Popov ghosts](../../../../faddeev-popov-ghost.md) interact with $h$ and **do not decouple for generic $\xi$**. The distinction from part [a](../a.md) is the scalar dependence of the [gauge fixing](../../../../gauge-fixing.md) function. In the $\xi\to0$ [Landau gauge](../../../../landau-gauge-for-a-uniform-magnetic-field.md) limit these particular ghost interactions vanish.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
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
