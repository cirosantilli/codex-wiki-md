<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put

$$
k=\frac{\omega}{c_0},\qquad
p=k\sin\theta_i,\qquad
q_0=k\cos\theta_i,
$$

and let $q_1=nk\cos\theta_T$ be the downward [vertical wavenumber](../../../../../../vertical-wavenumber.md) in the lower half-space. The given form of [Snell's law](../../../../../../snell-s-law.md) says

$$
q_1=q_0\sqrt{1+\alpha}.
$$

With the $e^{-i\omega t}$ convention, write the incident, reflected, and transmitted [plane waves](../../../../../../plane-wave.md) as

$$
\psi_i=e^{i(px-q_0z)},\qquad
\psi_r=R e^{i(px+q_0z)},\qquad
\psi_t=T e^{i(px-q_1z)}.
$$

The two [interface conditions](../../../../../../scalar-wave-interface-condition.md) at $z=0$ give

$$
1+R=T,
\qquad
q_0(1-R)=q_1T.
$$

Solving this [linear system](../../../../../../system-of-linear-equations.md) gives the [reflection and transmission coefficients at a scalar-wave interface](../../../../../../reflection-and-transmission-coefficients-at-a-scalar-wave-interface.md)

$$
\boxed{R=\frac{q_0-q_1}{q_0+q_1}
=\frac{1-\sqrt{1+\alpha}}{1+\sqrt{1+\alpha}}},
\qquad
\boxed{T=\frac{2q_0}{q_0+q_1}
=\frac{2}{1+\sqrt{1+\alpha}}}.
$$

Thus the exact fields are

$$
\boxed{\psi_0=e^{i(px-q_0z)}+R e^{i(px+q_0z)}}
\quad(z>0),
$$



$$
\boxed{\psi_1=T e^{i(px-q_1z)}}
\quad(z<0).
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
