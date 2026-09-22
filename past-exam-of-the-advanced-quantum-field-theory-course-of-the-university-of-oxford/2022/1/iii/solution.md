<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $s=(p_1+p_2)^2=m_h^2$, so $p_1^2=p_2^2=0$ and $p_1\cdot p_2=s/2$. The physical [polarization vectors](../../../../polarization-vector.md) obey $\epsilon_1\cdot p_1=\epsilon_2\cdot p_2=0$. Write $X_{\mu\nu}\simeq Y_{\mu\nu}$ when they agree after contraction with these [polarization vectors](../../../../polarization-vector.md); terms proportional to $p_{1,\mu}$ or $p_{2,\nu}$ may then be discarded.

The [gamma matrix trace identities](../../../../gamma-matrix-trace-identities.md) kill the terms with an odd number of [gamma matrices](../../../../gamma-matrices.md). The remaining three two-[momentum](../../../../momentum-split.md) terms and the term with three factors of $m$ are

$$
\begin{aligned}
\frac{T_{\mu\nu}}{4m}={}&m^2g_{\mu\nu}
+l_\mu(l-p_2)_\nu+(l-p_2)_\mu l_\nu-g_{\mu\nu}l\cdot(l-p_2)\\
&+l_\mu(l+p_1)_\nu+(l+p_1)_\mu l_\nu-g_{\mu\nu}l\cdot(l+p_1)\\
&+g_{\mu\nu}(l-p_2)\cdot(l+p_1)-(l-p_2)_\mu(l+p_1)_\nu+(l+p_1)_\mu(l-p_2)_\nu.
\end{aligned}
$$

In the $g_{\mu\nu}$ coefficient the terms linear in $l\cdot p_i$ cancel, leaving $m^2-l^2-s/2$. Among the other terms, the surviving mixed products of $l$ and $p_i$ also cancel. Consequently

$$
T_{\mu\nu}\simeq4m\left[4l_\mu l_\nu+p_{2,\mu}p_{1,\nu}+(m^2-s/2-l^2)g_{\mu\nu}\right].
$$

In the second [Feynman diagram](../../../../feynman-diagram.md), exchange the external labels and change the dummy [loop momentum](../../../../loop-momentum.md) $l\mapsto-l$. Its projected numerator and denominator become identical to those of the first [Feynman diagram](../../../../feynman-diagram.md). Hence

$$
\boxed{\mathcal M'_{\mu\nu}=8iN_cye^2Q^2m\int\frac{d^4l}{(2\pi)^4}
\frac{4l_\mu l_\nu+p_{2,\mu}p_{1,\nu}+(m^2-s/2-l^2)g_{\mu\nu}}{D_0D_1D_2}.}
$$

With the common factor $8m$ extracted, the primitive integer coefficients are

$$
\boxed{A=4,\qquad B=1,\qquad C=1,\qquad \text{prefactor}=8iN_c\frac{\lambda_t}{\sqrt2}e^2e_t^2m_t.}
$$

Equivalently, extracting only $m$ gives $(A,B,C)=(32,8,8)$ and prefactor $iN_c\lambda_te^2e_t^2m_t/\sqrt2$. A common rescaling of all three coefficients changes the prefactor inversely. The physical [scattering amplitude](../../../../scattering-amplitude.md) is $\epsilon_1^\mu\epsilon_2^\nu\mathcal M'_{\mu\nu}$; the projected integrand is not an identity for an arbitrary uncontracted off-shell [tensor](../../../../tensor.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the advanced quantum field theory course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory course of the University of Oxford](../../../../advanced-quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
