<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Common temporal phase requires a monomial in the first component to contain one more unbarred factor than barred factors. If the exponent differences for the two coordinates are $m_1,m_2$, then $m_1+m_2=1$. Equivariance under $\rho$ requires its spatial weight $-m_1+m_2$ to be $-1$ modulo three, hence $m_1\equiv1\pmod3$. Up to degree five, $m_1=1,m_2=0$ gives $z_1$ times all quadratic and quartic polynomials in the intensities $|z_1|^2,|z_2|^2$. The other possibility is $m_1=-2,m_2=3$, giving $\bar z_1^2z_2^3$ at degree five. No even-degree monomials satisfy the temporal weight.

Reflection determines the second component by exchanging indices. Thus the [dihedral threefold Hopf normal form](../../../../../../dihedral-threefold-hopf-normal-form.md), through fifth order, is

$$
\boxed{\begin{aligned}
\dot z_1={}&z_1\left[\alpha+a|z_1|^2+b|z_2|^2+c|z_1|^4+d|z_1|^2|z_2|^2+e|z_2|^4\right]+f\bar z_1^2z_2^3,\\
\dot z_2={}&z_2\left[\alpha+a|z_2|^2+b|z_1|^2+c|z_2|^4+d|z_1|^2|z_2|^2+e|z_1|^4\right]+f\bar z_2^2z_1^3,
\end{aligned}}
$$

with complex coefficients, $\alpha=\mu+i\omega_0$ at leading parameter order, and higher spatial-degree terms omitted. Coefficients may vary smoothly with the bifurcation parameter. The phase-sensitive quintic is allowed by the discrete threefold rotation, even though continuous independent rotations of the two coordinates would forbid it.

For a rotating wave, substitute $(z_1,z_2)=(re^{i\Omega t},0)$. Its component amplitude and frequency obey

$$
0=\mu+a_Rr^2+c_Rr^4,\qquad
\Omega=\omega_0+a_Ir^2+c_Ir^4.
$$

Here subscripts denote real and imaginary parts. For a standing wave, substitute $(z_1,z_2)=(re^{i\Omega t},\sigma re^{i\Omega t})$, with $\sigma=\pm1$. The resonant term becomes $\sigma f r^5e^{i\Omega t}$ in the first component, and reflection ensures the second component agrees. Therefore

$$
0=\mu+(a_R+b_R)r^2+(c_R+d_R+e_R+\sigma f_R)r^4,
$$



$$
\Omega=\omega_0+(a_I+b_I)r^2+(c_I+d_I+e_I+\sigma f_I)r^4.
$$

Set $A_s=a_R+b_R$ and $B_\sigma=c_R+d_R+e_R+\sigma f_R$. For constant leading coefficients, solving for $r^2$ gives

$$
\boxed{\begin{aligned}
r_{\mathrm{rot}}^2&=-\frac\mu{a_R}-\frac{c_R\mu^2}{a_R^3}+O(\mu^3),\\
r_\sigma^2&=-\frac\mu{A_s}-\frac{B_\sigma\mu^2}{A_s^3}+O(\mu^3).
\end{aligned}}
$$

Smooth parameter dependence adds common higher corrections but does not remove the generic difference between the two standing families. The rotating and standing component amplitudes differ already at cubic order unless their coefficient combinations accidentally agree. The standing waves have the same cubic amplitude, but

$$
\boxed{r_+^2-r_-^2=-\frac{2f_R\mu^2}{A_s^3}+O(\mu^3),}
$$

which is generically nonzero. Thus **all three branch types generically have different amplitudes**, with the distinction between the standing families first visible at fifth order. In total Euclidean norm the rotating wave has amplitude $r_{\mathrm{rot}}$, whereas each standing wave has amplitude $\sqrt2\,r_\sigma$. The relevant branches exist on the parameter sides making their small squared amplitudes positive; nonzero cubic coefficients are part of the generic Hopf assumptions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
