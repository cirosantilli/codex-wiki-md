<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A constant-amplitude [plane wave](../../../../../../plane-wave.md) has no density derivative and therefore no damping. The complete family is

$$
\boxed{\psi=A\exp[i(\mathbf k\cdot\mathbf x-\omega t+\chi)],
\qquad\omega=\frac{k^2}{2}+A^2-1,\qquad A\ge0,}
$$

with arbitrary constant phase $\chi$. The background in the question is the member $A=1$.

Use the exact amplitude–phase equations derived above with $\mathbf v_n=0$. To first order in the perturbation, $\rho=1+2\epsilon R$ and $\mathbf v_s=\mathbf k+\epsilon\nabla\Theta$, so

$$
(\partial_t+\mathbf k\cdot\nabla)R=-\frac12\nabla^2\Theta,
$$



$$
(\partial_t+\mathbf k\cdot\nabla)\Theta
=\frac12\nabla^2R-2R-2\zeta R_t.
$$

These equations retain the [quantum potential](../../../../../../quantum-potential.md) contribution because no long-wavelength truncation is assumed in this subpart. In particular damping contains $R_t$, not the advective derivative along the moving condensate: its reference is the stationary [normal fluid](../../../../../../normal-component-of-a-superfluid.md).

For the proposed periodic perturbation, write $q=\mathbf k\cdot\mathbf l$ and $L=l^2$. The amplitude coefficients satisfy

$$
\begin{pmatrix}
\sigma+iq&-L/2\\
2+L/2+2\zeta\sigma&\sigma+iq
\end{pmatrix}
\begin{pmatrix}R_0\\\Theta_0\end{pmatrix}=0.
$$

A nonzero perturbation therefore requires the [plane-wave dispersion of a material-density-damped condensate](../../../../../../plane-wave-dispersion-of-a-material-density-damped-condensate.md)

$$
\boxed{(\sigma+iq)^2+\zeta l^2\sigma+l^2+\frac{l^4}{4}=0,}
$$

or equivalently $\sigma^2+(2iq+\zeta l^2)\sigma+l^2+l^4/4-q^2=0$. At zero background flow the roots are $-\zeta l^2/2\pm\sqrt{\zeta^2l^4/4-l^2-l^4/4}$, whose real parts are negative for $l\ne0$. As $\zeta\to0$, $\sigma=-iq\pm i\sqrt{l^2+l^4/4}$ recovers the advected [Bogoliubov spectrum](../../../../../../bogoliubov-quasiparticle-dispersion.md) with long-wavelength [sound speed](../../../../../../speed-of-sound.md) one in these units. This differs from question 1's time normalization, whose [sound speed](../../../../../../speed-of-sound.md) is $1/\sqrt2$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
