<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $V=r\partial_r$, [Cartan's magic formula](../../../../../../../cartan-s-magic-formula.md) gives

$$
\mathcal L_Vdr=d(i_Vdr)+i_Vd(dr)=d(r)=dr,
$$

whereas contraction and exterior differentiation both vanish for $du,d\theta,d\phi$. Thus

$$
\mathcal L_Vdu=\mathcal L_Vd\theta=\mathcal L_Vd\phi=0.
$$

Applying the [Lie derivative](../../../../../../../lie-derivative-of-a-differential-form.md) to  
$g=-du^2-2,du,dr+r^2d\Omega^2$ yields

$$
\mathcal L_Vg=-2,du,dr+2r^2d\Omega^2.
$$

Here $n_a=-(du+dr)_a$ and $V_a=-r(du)_a$, so comparison with $2g$ gives

$$
\boxed{(\mathcal L_Vg)_{ab}
=2g_{ab}+\frac2r n_{(a}V_{b)}},
\qquad \boxed{\alpha=2}.
$$

Using tracelessness from part (b)(i),

$$
\nabla_a(T^{ab}V_b)
=\frac1rT^{ab}n_aV_b\geq0
$$

by the [dominant energy condition](../../../../../../../dominant-energy-condition.md), because $n$ is future timelike and $V$ is future null.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 309](../../../../paper-309-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
