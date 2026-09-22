<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the [poloidal magnetic flux function](../../../../../poloidal-magnetic-flux-function.md) and toroidal amplitude explicitly in spherical components:

$$
B_r=\frac{\chi_\theta}{r^2\sin\theta},\qquad B_\theta=-\frac{\chi_r}{r\sin\theta},\qquad B_\phi=\frac{\psi}{r\sin\theta}.
$$

Dotting the [magnetostatic equilibrium](../../../../../magnetostatic-equilibrium.md) equation with $\mathbf B$ gives $\mathbf B\cdot\nabla p=0$. Since all fields are axisymmetric, the [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) is tangent to the contours of $\chi$ in a meridional section. Thus, locally on regular connected flux surfaces, $p=p(\chi)$. This is a local flux-surface statement; disconnected surfaces with the same numerical value of $\chi$ need not have the same pressure without further global assumptions.

Taking the azimuthal component of the [Lorentz force](../../../../../lorentz-force.md) gives

$$
[(\nabla\times\mathbf B)\times\mathbf B]_\phi=\frac{\psi_r\chi_\theta-\psi_\theta\chi_r}{r^3\sin^2\theta}=0.
$$

Its numerator is the meridional [Jacobian determinant](../../../../../jacobian-determinant.md) of $\psi$ and $\chi$. Vanishing therefore implies locally $\psi=\psi(\chi)$ on the same regular surfaces. Define

$$
\Delta_*\chi=\chi_{rr}+\frac{\sin\theta}{r^2}\partial_\theta\left(\frac{\chi_\theta}{\sin\theta}\right).
$$

A direct curl calculation now gives

$$
\nabla\times\mathbf B=\psi'(\chi)\mathbf B_{\rm pol}-\frac{\Delta_*\chi}{r\sin\theta}\mathbf e_\phi.
$$

Since $\mathbf e_\phi\times\mathbf B_{\rm pol}=\nabla\chi/(r\sin\theta)$, the remaining force is

$$
(\nabla\times\mathbf B)\times\mathbf B=-\frac{\Delta_*\chi+\psi\psi'}{r^2\sin^2\theta}\nabla\chi.
$$

Consequently the [spherical magnetostatic pressure balance](../../../../../spherical-magnetostatic-pressure-balance.md) equation following from the stated physical force balance is

$$
\boxed{\Delta_*\chi+\psi\frac{d\psi}{d\chi}=-\mu_0r^2\sin^2\theta\frac{dp}{d\chi}.}
$$

**The PDF's displayed scalar equation has the wrong sign and omits $\mu_0$ for its stated pressure p.** This is not corrected by setting $\mu_0=1$, which leaves the sign discrepancy. For example, $\chi=r^4\sin^2\theta$, $\psi=0$, $p=p_0-10\chi/\mu_0$ satisfies the stated vector force balance and the corrected scalar equation, because $\Delta_*\chi=10r^2\sin^2\theta$; it fails the printed scalar equation. One could obtain the printed form by replacing its pressure variable by $-\mu_0p_{\rm physical}$, but that is not the variable in the given force balance.

Now set $\psi=\alpha\chi$, $p=p_0+P\chi$, and $\chi=F(r)\sin^2\theta$. The angular operator gives $-2F\sin^2\theta/r^2$, so

$$
F''+\left(\alpha^2-\frac2{r^2}\right)F=-\mu_0P r^2.
$$

For the trigonometric form in the question, direct substitution yields

$$
F=A\cos\alpha r+B\frac{\sin\alpha r}{r}+cr^2\quad\Longrightarrow\quad F''+\left(\alpha^2-\frac2{r^2}\right)F=-\frac{2(A+\alpha B)}{r^2}\cos\alpha r+\alpha^2cr^2.
$$

For $\alpha\ne0$, this is a solution provided

$$
\boxed{B=-\frac A\alpha,\qquad P=-\frac{\alpha^2c}{\mu_0}.}
$$

The same coefficient relation makes the trigonometric pair regular at the origin: $\cos\alpha r-\sin\alpha r/(\alpha r)=-\alpha^2r^2/3+O(r^4)$. Thus all components of the [magnetic field](../../../../../magnetic-field.md) are finite there. With $p_0=0$, this explicitly constructs the requested proportional-pressure family; adding $p_0$ does not change force balance. The coefficient c is the one called C in the final sentence of the PDF.

For a [confined linear-pressure spherical magnetic equilibrium](../../../../../confined-linear-pressure-spherical-magnetic-equilibrium.md), the condition that the entire [magnetic field](../../../../../magnetic-field.md) vanish on $r=a$ is precisely $F(a)=F'(a)=0$. In components these conditions read

$$
A\cos x+\frac B a\sin x+ca^2=0,\qquad -A\alpha\sin x+B\left(\frac\alpha a\cos x-\frac1{a^2}\sin x\right)+2ca=0,\qquad x=\alpha a.
$$

They eliminate both the radial and meridional components; the toroidal component vanishes too because $\psi=\alpha\chi$. For a nontrivial solution with $A\ne0$, substituting $B=-A/\alpha$ gives

$$
\boxed{c=-\frac A{a^2}\left(\cos x-\frac{\sin x}{x}\right),\qquad (x^2-3)\sin x+3x\cos x=0.}
$$

The last equation selects the allowed nonzero values of $\alpha a$. Equivalently, when division is legitimate, $\tan x=3x/(3-x^2)$; the undivided equation also handles vanishing denominators correctly. Since $\chi(a,\theta)=0$, **$\boxed{p(a,\theta)=p_0}$** is independent of latitude. In the strictly proportional convention $p=P\chi$, this is zero. The zero-field solution is a trivial possibility; the displayed conditions describe the nontrivial confined family.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
