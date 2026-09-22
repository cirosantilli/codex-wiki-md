<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There are two normalization problems in the printed energy identity. In [conformal time](../../../../../../../conformal-time.md), the physical density of a homogeneous scalar is $T_{00}/a^2$, and its kinetic contribution contains $\phi'^2$, not one power of $\phi'$. The [conformal density of a canonical scalar field](../../../../../../../conformal-density-of-a-canonical-scalar-field.md) follows directly from the [stress-energy tensor](../../../../../../../stress-energy-tensor.md):

$$
\rho_\phi=\frac{\phi'^2}{2a^2}+V,\qquad
p_\phi=\frac{\phi'^2}{2a^2}-V,\qquad T_{00}=a^2\rho_\phi.
$$

Writing $K=\phi'^2/(2a^2)$, the condition $K-V=-(K+V)/3$ gives $V=2K$, hence

$$
\boxed{K=\rho_\phi/3,\qquad V=2\rho_\phi/3,\qquad
\phi'^2=\frac{2a^2\rho_\phi}{3}=\frac{2T_{00}}3.}
$$

The reconstruction is consistent with this corrected identity; the unsquared printed identity cannot hold as an energy relation.

The [constant-equation-of-state density scaling](../../../../../../../constant-equation-of-state-density-scaling.md) for this [coasting fluid](../../../../../../../coasting-fluid.md) gives $\rho_\phi=\rho_{X0}a^{-2}$, where $\rho_{X0}=3M^2H_0^2\Omega_X$. Choose the branch on which $\phi$ increases. Then

$$
\phi'=\sqrt2MH_0\sqrt{\Omega_X},\qquad
V=\frac{2M^2H_0^2\Omega_X}{a^2}.
$$

Keeping all three density parameters explicitly, the [Friedmann equations](../../../../../../../friedmann-equations.md) in [conformal time](../../../../../../../conformal-time.md) give

$$
a'^2=H_0^2\left(\Omega_r+\Omega_ma+\Omega_Xa^2\right),\qquad
\frac{da}{d\phi}=\frac1{\sqrt2M}
\sqrt{a^2+\frac{\Omega_m}{\Omega_X}a+\frac{\Omega_r}{\Omega_X}}.
$$

For $\Omega_X>0$, define

$$
b=\frac{\Omega_m}{2\Omega_X},\qquad
A=\frac{\sqrt{\Omega_m^2/4-\Omega_r\Omega_X}}{\Omega_X}.
$$

The square root is $\sqrt{(a+b)^2-A^2}$. Integrating on the expanding branch gives

$$
\operatorname{arcosh}\frac{a+b}{A}
=\frac{\phi-\phi_0}{\sqrt2M}+C,
$$

where $a(\phi_0)=1$. Thus the [scalar-field reconstruction of a coasting component](../../../../../../../scalar-field-reconstruction-of-a-coasting-component.md) is

$$
\boxed{a=A\cosh[B(\phi-\phi_0)+C]+D,\quad
B=\frac1{\sqrt2M}=\frac{\sqrt{4\pi}}{m_{\rm pl}},\quad
C=\operatorname{arcosh}\frac{1+b}{A},\quad D=-b.}
$$

Substitution into the potential gives the requested present-field parametrization:

$$
\boxed{V(\phi)=\frac{2M^2H_0^2\Omega_X}
{\left[A\cosh\left(\frac{\phi-\phi_0}{\sqrt2M}+C\right)-b\right]^2}.}
$$

The domain is the branch where $a>0$ and the hyperbolic argument is positive; reversing the direction of the field changes the sign of $B$. The actual discriminant condition is $\Omega_m^2/4>\Omega_r\Omega_X$. The supplied stronger bound suffices for physical density fractions $0<\Omega_X\le1$. No density parameter has been eliminated using the flatness sum.

As a check, $\phi'$ is constant and $V_{,\phi}=-2V(a'/a)/\phi'$. Since $a^2V=\phi'^2$ along this solution, $\phi''+2(a'/a)\phi'+a^2V_{,\phi}=0$ identically. The reconstructed field therefore satisfies its equation of motion as well as the [Friedmann equations](../../../../../../../friedmann-equations.md) and required [equation of state](../../../../../../../equation-of-state.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 70](../../../../paper-70-split.md)
5. [Iii](../../../../split.md)
6. [2001](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
