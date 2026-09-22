<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Galerkin method](../../../../../../galerkin-method.md), rather than pointwise equality: products generate harmonics outside the retained five-dimensional space. Put $X=\alpha x$, $Z=\pi z$, and denote the five prefactors by

$$
P={2\sqrt2\beta\over\alpha}a,\quad T={2\sqrt2\over\beta}b,\quad C=-c/\pi,\quad
D={2\sqrt2\pi\over\alpha\beta}d,\quad E=e/\alpha.
$$

The retained [streamfunction](../../../../../../stream-function.md) is $P\sin X\sin Z$, the retained temperature perturbation is $T\cos X\sin Z+C\sin2Z$, and the retained magnetic-flux perturbation is $D\sin X\cos Z+E\sin2X$. These satisfy all the stated boundary conditions. Let $J(f,g)=f_xg_z-f_zg_x$, the [streamfunction advection bracket](../../../../../../streamfunction-advection-bracket.md). [Orthogonality](../../../../../../orthogonal-vectors.md) of the [sine](../../../../../../sine.md) and [cosine](../../../../../../cosine.md) modes gives the following coefficients of the retained harmonics:

$$
\begin{aligned}
J(\psi,\Delta\psi)&=0,\\
[J(\psi,\theta)]_{\cos X\sin Z}&=-\alpha\pi PC=\alpha Pc,\\
[J(\psi,\theta)]_{\sin2Z}&=\alpha\pi PT/2,\\
[J(\psi,A)]_{\sin X\cos Z}&=\alpha\pi PE,\\
[J(\psi,A)]_{\sin2X}&=-\alpha\pi PD/2,\\
[J(A,\Delta A)]_{\sin X\sin Z}&=\alpha\pi DE(3\alpha^2-\pi^2).
\end{aligned}
$$

For example the $C$ contribution to the temperature bracket is $\alpha\pi PC[\cos X\sin3Z-\cos X\sin Z]$. The magnetic bracket follows by writing $A=A_D+A_E$: $J(A,\Delta A)=(\beta^2-4\alpha^2)J(A_D,A_E)$ and $J(A_D,A_E)=\alpha\pi DE(\sin3X-\sin X)\sin Z$. These identities exhibit both the retained terms and discarded harmonics.

Before rescaling time, the projected coefficient equations are

$$
\begin{aligned}
-\beta^2\dot P&=\sigma\beta^4P-\sigma rR_0\alpha T+\sigma\zeta Q[\beta^2\pi D+\alpha\pi DE(3\alpha^2-\pi^2)],\\
\dot T+\alpha Pc&=-\beta^2T+\alpha P,\\
-\dot c/\pi+\alpha\pi PT/2&=4\pi c,\\
\dot D+\alpha\pi PE&=-\zeta\beta^2D+\pi P,\\
\dot E-\alpha\pi PD/2&=-4\zeta\alpha^2E.
\end{aligned}
$$

Substitute the prefactors and divide time derivatives by $\beta^2$. With $\tau=\beta^2t$, $\varpi=4\pi^2/\beta^2$ and $q=\pi^2Q/\beta^4$, the resulting [five-mode vertical-field magnetoconvection](../../../../../../five-mode-vertical-field-magnetoconvection.md) equations are

$$
\boxed{\begin{aligned}
a'&=-\sigma a+\sigma rb-\sigma\zeta qd-\sigma\zeta q(3-\varpi)ed,\\
b'&=a-b-ac,\\c'&=\varpi(-c+ab),\\
d'&=a-\zeta d-ae,\\e'&=-(4-\varpi)\zeta e+\varpi ad.
\end{aligned}}
$$

Here primes denote differentiation in $\tau$. The factor $3-\varpi$ is $(3\alpha^2-\pi^2)/\beta^2$, which checks the magnetic nonlinear sign. There is a terminology qualification in the source: on this thermal diffusion time scale, its $\zeta$ is the [magnetic-to-thermal diffusivity ratio](../../../../../../magnetic-to-thermal-diffusivity-ratio.md) $\eta/\kappa$. The conventional [magnetic Prandtl number](../../../../../../magnetic-prandtl-number.md) is $\nu/\eta=\sigma/\zeta$, where $\sigma$ is the [Prandtl number](../../../../../../prandtl-number.md). The displayed equations and subsequent calculation use the source's $\zeta$ unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
