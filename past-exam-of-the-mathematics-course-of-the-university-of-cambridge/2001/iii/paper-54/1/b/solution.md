<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The degree-five row of the [wavevector selection rule for equivariant monomials](../../../../../../wavevector-selection-rule-for-equivariant-monomials.md) in part (a) has two vectors other than $(1,0,0,0)$. They correspond exactly to

$$
\boxed{\overline A_2A_3^2A_4^2,\qquad \overline A_1A_2^2A_3\overline A_4.}
$$

The vector $(1,0,0,0)$ gives only regular fifth-order terms $A_1|A_j|^2|A_k|^2$. Omitting those as required, and applying the same two square-symmetry generators, the truncated [normal form of a dynamical system](../../../../../../normal-form-dynamical-systems.md) is

$$
\begin{aligned}
\dot A_1&=A_1G_1+e\overline A_2A_3^2A_4^2+f\overline A_1A_2^2A_3\overline A_4,\\
\dot A_2&=A_2G_2+e\overline A_1A_4^2A_3^2+f\overline A_2A_1^2A_4\overline A_3,\\
\dot A_3&=A_3G_3+eA_4A_1^2\overline A_2^{\,2}+f\overline A_3\overline A_4^{\,2}A_1A_2,\\
\dot A_4&=A_4G_4+eA_3A_2^2\overline A_1^{\,2}+f\overline A_4\overline A_3^{\,2}A_2A_1.
\end{aligned}
$$

Here $e,f$ are real because rotation by $\pi$ acts by [complex conjugation](../../../../../../complex-conjugation.md). These are equations for steady patterns, so all four complex right-hand sides must vanish; constancy of the two invariant angles alone would only establish a [relative equilibrium](../../../../../../relative-equilibrium.md) and could allow translation drift.

Take a nonzero equal-magnitude state, $|A_j|=R>0$, and set $z=R^2$, $S=c_1+c_2+c_3+c_4$, $\rho=\sigma+Sz$. Dividing each equation by its nonzero [amplitude](../../../../../../wave-amplitude.md) gives, in order,

$$
\begin{aligned}
0&=\rho+z^2(e e^{-i\chi_2}+f e^{-i\chi_1}),\\
0&=\rho+z^2(e e^{-i\chi_2}+f e^{ i\chi_1}),\\
0&=\rho+z^2(e e^{ i\chi_1}+f e^{ i\chi_2}),\\
0&=\rho+z^2(e e^{-i\chi_1}+f e^{ i\chi_2}).
\end{aligned}
$$

Taking [imaginary parts](../../../../../../imaginary-part.md), adding and subtracting pairs, yields

$$
e\sin\chi_2=f\sin\chi_1=e\sin\chi_1=f\sin\chi_2=0.
$$

Thus, unless $e=f=0$, each invariant [phase](../../../../../../phase-waves.md) is zero or $\pi$ modulo $2\pi$. Equality of the [real parts](../../../../../../real-part.md) further gives

$$
(e-f)(\cos\chi_1-\cos\chi_2)=0.
$$

This identifies the [equal-amplitude states of an eight-mode square pattern](../../../../../../equal-amplitude-states-of-an-eight-mode-square-pattern.md) completely. For generic $e\ne f$, the two nonzero [phase](../../../../../../phase-waves.md) types, with their [amplitude](../../../../../../wave-amplitude.md) equations, are

$$
\boxed{\begin{array}{c|c}
(\chi_1,\chi_2)&\text{equation for }z>0\\\hline
(0,0)&\sigma+Sz+(e+f)z^2=0\\
(\pi,\pi)&\sigma+Sz-(e+f)z^2=0.
\end{array}}
$$

Representatives are respectively $(A_1,A_2,A_3,A_4)=R(1,1,1,1)$ and $R(-1,1,-1,1)$. Spatial translations change individual [phases](../../../../../../phase-waves.md) but leave the indicated [phase](../../../../../../phase-waves.md) pair fixed. [Reflection](../../../../../../reflection-mathematics.md) acts on the invariant angles as $(\chi_1,\chi_2)\mapsto(-\chi_1,\chi_2)$, and interchange of $x,y$ as $(\chi_1,\chi_2)\mapsto(-\chi_2,-\chi_1)$. Thus the two rows are not equivalent under square [symmetry](../../../../../../symmetry-physics.md) and translations. Every positive root of the corresponding [polynomial](../../../../../../polynomial-split.md) gives an [amplitude](../../../../../../wave-amplitude.md) branch of that type; if there is no positive root, that type is absent at those parameter values.

There are two [coefficient](../../../../../../coefficient.md) degeneracies to include. When $e=f\ne0$, the mixed pairs $(0,\pi)$ and $(\pi,0)$ are allowed and are equivalent under square [symmetry](../../../../../../symmetry-physics.md). They form **one additional [phase](../../../../../../phase-waves.md) type**, with [amplitude](../../../../../../wave-amplitude.md) equation $\boxed{\sigma+Sz=0}$; $iR(1,1,1,1)$ is a representative. When $e=f=0$, all invariant [phases](../../../../../../phase-waves.md) are unrestricted, and the same cubic [amplitude](../../../../../../wave-amplitude.md) equation gives a continuous family modulo translations and the finite square-group action. Even if $e+f=0$ but $e\ne f$, only the original two [phase](../../../../../../phase-waves.md) types remain: the equality of their [amplitude](../../../../../../wave-amplitude.md) equations does not remove the [phase](../../../../../../phase-waves.md) constraints. Finally, the all-zero state is always a separate steady state and has no defined polar [phases](../../../../../../phase-waves.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
