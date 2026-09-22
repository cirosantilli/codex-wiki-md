<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The contrast is weak: $(n_1-n_2)/n_2=0.01$. Use a scalar weak-guidance [Helmholtz equation](../../../../helmholtz-equation.md) for a transverse field component, with longitudinal [wave number](../../../../wavenumber.md) $b$ and vacuum [wave number](../../../../wavenumber.md) $k_0=2\pi/\lambda_0$. Separating variables as $\psi=F_l(r)e^{il\phi}e^{ibz}$ gives

$$
F_l''+\frac1rF_l'+\left(n^2k_0^2-b^2-\frac{l^2}{r^2}\right)F_l=0.
$$

A bound mode requires $n_2k_0<b<n_1k_0$. Define

$$
u=a\sqrt{n_1^2k_0^2-b^2},\qquad
w=a\sqrt{b^2-n_2^2k_0^2},\qquad
V^2=u^2+w^2=a^2k_0^2(n_1^2-n_2^2).
$$

The [step-index fiber normalized frequency](../../../../step-index-fiber-normalized-frequency.md) is $V$; $u$ is a dimensionless core transverse [wave number](../../../../wavenumber.md). Regularity at $r=0$ selects the [Bessel function of the first kind](../../../../bessel-function-of-the-first-kind.md), while decay at infinity selects the [Modified Bessel function of the second kind](../../../../modified-bessel-function-of-the-second-kind.md):

$$
F_l(r)=\begin{cases}A J_l(ur/a),&r<a,\\B K_l(wr/a),&r>a.\end{cases}
$$

In this scalar approximation, continuity of the field and its radial derivative gives

$$
A J_l(u)=B K_l(w),\qquad
A uJ_l'(u)=B wK_l'(w),\qquad
\frac{uJ_l'(u)}{J_l(u)}=\frac{wK_l'(w)}{K_l(w)}.
$$

At cutoff the [evanescent wave](../../../../evanescent-wave.md) extends arbitrarily far into the cladding, so $b\downarrow n_2k_0$, $w\downarrow0$ and $u\to V$. For the first azimuthally varying family $l=1$, the recurrence relations reduce the last equality to

$$
\frac{uJ_0(u)}{J_1(u)}=-\frac{wK_0(w)}{K_1(w)}.
$$

As $w\to0$, $K_1(w)\sim1/w$ and $K_0(w)\sim-\ln w$, making the right side tend to zero. Thus the onset is at the first positive zero of $J_0$:

$$
\boxed{V_c=j_{0,1}=2.404825\ldots\simeq2.4,\qquad
2\pi a\sqrt{n_1^2-n_2^2}>2.4\lambda_0.}
$$

The scalar $l=0$ fundamental family has no positive cutoff. The first additional spatial family is the $l=1$ family just found; the next radial $l=0$ and first $l=2$ families require the larger zero $j_{1,1}\simeq3.832$. This establishes the first multimode boundary rather than merely finding one possible cutoff. The two polarizations of the fundamental family are not counted as two spatial modes. Exact vector interface conditions split some higher-mode degeneracies at finite contrast; the displayed condition is the weak-guidance result intended by the supplied scalar equations.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
