<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

At one loop, writing $t=\log\mu$ makes the [renormalization-group beta function](../../../../../beta-function-physics.md) $dg_i/dt=b_i g_i^3$. For $b_i>0$ a positive [running coupling](../../../../../running-coupling.md) grows towards high energies and decreases towards the infrared. Extrapolation of the one-loop expression gives a finite ultraviolet [Landau pole](../../../../../landau-pole.md); perturbation theory fails before it reaches that pole. For $b_i<0$, the coupling decreases towards high energies, giving [asymptotic freedom](../../../../../asymptotic-freedom.md), and grows towards the infrared. The formal infrared pole identifies a [strong-coupling scale](../../../../../strong-coupling-scale.md), where the weak-coupling approximation no longer applies. These conclusions concern the small-coupling branch; a pole in the perturbative solution does not establish a pole in the exact theory. If $b_i=0$, higher-order terms decide the running.

From $\alpha_i=g_i^2/(4\pi)$,

$$
\frac{d\alpha_i}{d\log\mu}=8\pi b_i\alpha_i^2,
\qquad \frac{d\alpha_i^{-1}}{d\log\mu}=-8\pi b_i.
$$

Integrating the one-loop [beta function](../../../../../beta-function-physics.md) gives

$$
\boxed{\alpha_i^{-1}(\mu)=\alpha_i^{-1}(m_Z)-8\pi b_i\log\frac\mu{m_Z},\qquad
\alpha_i(\mu)=\frac{\alpha_i(m_Z)}{1-8\pi b_i\alpha_i(m_Z)\log(\mu/m_Z)}.}
$$

These formulas retain the same particle content and neglect threshold corrections throughout the interval. For $b_i>0$, the formal pole is $\mu=m_Z\exp[1/(8\pi b_i\alpha_i(m_Z))]$; for $b_i<0$ the analogous scale lies below $m_Z$.

For [one-loop normalized hypercharge unification](../../../../../one-loop-normalized-hypercharge-unification.md), the normalized hypercharge coupling is $\alpha_Y^{\mathrm{GUT}}=(5/3)\alpha_1$, so its inverse and one-loop slope are $(3/5)\alpha_1^{-1}$ and $(3/5)b_1$. Define

$$
U_1=\frac35\alpha_1^{-1}(m_Z),\quad U_2=\alpha_2^{-1}(m_Z),\quad U_3=\alpha_3^{-1}(m_Z),\quad
L_G=\log\frac{M_{\mathrm{GUT}}}{m_Z}.
$$

Equality of the three normalized inverses at the unification scale gives

$$
U_1-U_2=8\pi\left(\frac35b_1-b_2\right)L_G,\qquad
U_3-U_2=8\pi(b_3-b_2)L_G.
$$

Eliminating $L_G$ proves

$$
\boxed{\alpha_3^{-1}(m_Z)=\alpha_2^{-1}(m_Z)+
\frac{b_3-b_2}{(3/5)b_1-b_2}
\left[\frac35\alpha_1^{-1}(m_Z)-\alpha_2^{-1}(m_Z)\right].}
$$

This expression assumes $(3/5)b_1\ne b_2$. If these slopes coincide, unification first requires $U_1=U_2$, and the displayed division is unavailable. A unification scale above $m_Z$ additionally requires the inferred $L_G$ to be positive. The relation is a consistency condition under the stated one-loop assumptions, not proof that the measured couplings unify without threshold effects.

For the two-loop [running coupling](../../../../../running-coupling.md), the claimed logarithmic asymptotic concerns the [asymptotically free](../../../../../asymptotic-freedom.md) branch with $\beta_0>0$ and $\mu/\Lambda\to\infty$. Set

$$
y=a^{-1},\qquad c=\frac{\beta_1}{\beta_0},\qquad L=\log\frac\mu\Lambda.
$$

The differential equation becomes $dy/dL=\beta_0+\beta_1/y=\beta_0(1+c/y)$. Separating variables yields

$$
y-c\log|y+c|=\beta_0L+K.
$$

A change of the [strong-coupling scale](../../../../../strong-coupling-scale.md) $\Lambda$ absorbs any additive constant $K$. Choose that scale so that $K=-c\log\beta_0$. On the large positive-$y$ branch the exact implicit relation is then

$$
y-c\log\frac{y+c}{\beta_0}=\beta_0L.
$$

It first gives $y\sim\beta_0L$. Substituting this back into the logarithm gives $y=\beta_0L+c\log L+o(1)$. To determine the error rather than assume it, write $y=\beta_0L+c\log L+r(L)$. Expansion of the exact implicit relation yields

$$
r(L)=\frac{c\,[c\log L+c+r(L)]}{\beta_0L}
+O\!\left(\frac{(\log L)^2}{L^2}\right)
=\frac{c^2}{\beta_0}\frac{\log L+1}{L}
+O\!\left(\frac{(\log L)^2}{L^2}\right).
$$

Consequently the mathematically correct two-loop asymptotic is

$$
\boxed{a^{-1}(\mu)=\beta_0L+\frac{\beta_1}{\beta_0}\log L
+O\!\left(\frac{\log L}{L}\right).}
$$

More precisely, the next term is $\boxed{\beta_1^2(\log L+1)/(\beta_0^3L)}$. For $\beta_1\ne0$ this is not $O(1/L)$: multiplying the remainder by $L$ makes it grow as $(\beta_1^2/\beta_0^3)\log L$. No fixed change of $\Lambda$ can remove this term. Such a change adds a constant to $L$ and changes only constant or $1/L$ contributions, rather than the coefficient of $\log L/L$. Thus the two leading terms requested are correct, but the literal remainder printed in the PDF is too small. This is the [two-loop inverse-coupling logarithmic remainder](../../../../../two-loop-inverse-coupling-logarithmic-remainder.md).

If $\beta_1=0$, the one-loop result $y=\beta_0L$ is exact after choosing $\Lambda$. If $\beta_0=0$, the displayed expansion is undefined and the differential equation instead gives $y^2=2\beta_1\log\mu+\text{constant}$. For $\beta_0<0$, a positive weak coupling does not approach zero at arbitrarily large $\mu$ along the branch used above. The asymptotic assumptions therefore matter as well as the remainder.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
