<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The truncated fields must be interpreted as a [Galerkin method](../../../../../galerkin-method.md) approximation: project each equation onto its retained spatial modes and discard orthogonal higher harmonics. They are not an exact pointwise solution of the full partial differential equations, because the nonlinear terms generate additional harmonics. Write $X=kx$, $Z=\pi z$, and abbreviate the printed normalizations by

$$
S=\frac{\sqrt{8p}}k,\qquad T=\sqrt{\frac8p},\qquad D=\frac{\pi T}k,\qquad E=\frac1k.
$$

Then $\psi=Sa\sin X\sin Z$, $\theta=Tb\cos X\sin Z-c\sin2Z/\pi$, and $\chi=Dd\sin X\cos Z+Ee\sin2X$. All five amplitudes a,b,c,d,e depend on $\tau=pt$. Use the spatial [Jacobian determinant](../../../../../jacobian-determinant.md) $J(F,G)=F_xG_z-F_zG_x$ and the inner product over the stated rectangle. Orthogonality of the trigonometric modes makes projection equivalent to retaining their coefficients. In particular, $\nabla^2\psi=-p\psi$, so $J(\psi,\nabla^2\psi)=0$.

For the temperature equation, direct products give

$$
J(\psi,Tb\cos X\sin Z)=\frac{k\pi ST}{2}ab\sin2Z=4\pi ab\sin2Z.
$$

The other temperature contribution is $-2kSac\cos X\sin Z\cos2Z$. Since $\sin Z\cos2Z=(\sin3Z-\sin Z)/2$, its retained component is $kSac\cos X\sin Z$. Thus the projected temperature equation is

$$
pT\dot b=-pTb+kSa-kSac,\qquad -\frac p\pi\dot c+4\pi ab=4\pi c.
$$

Here the dot denotes $d/d\tau$. Since $kS/(pT)=1$ and $\varphi=4\pi^2/p$, these equations give $\dot b=-b+a(1-c)$ and $\dot c=\varphi(-c+ab)$.

Similarly, the two magnetic-advection products are

$$
J(\psi,Dd\sin X\cos Z)=-\frac{k\pi SD}{2}ad\sin2X=-\frac{4\pi^2}{k}ad\sin2X,
$$

while $J(\psi,Ee\sin2X)=-2\pi Sae\sin X\cos Z\cos2X$ has retained component $\pi Sae\sin X\cos Z$. The projected induction equation is therefore

$$
pD\dot d=\pi Sa-\zeta pDd-\pi Sae,\qquad pE\dot e=-4\zeta k^2Ee+\frac{4\pi^2}{k}ad.
$$

Using $\pi S/(pD)=1$ and $4k^2/p=4-\varphi$ gives $\dot d=-\zeta d+a(1-e)$ and $\dot e=-(4-\varphi)\zeta e+\varphi ad$.

It remains to project the [Lorentz force](../../../../../lorentz-force.md) in the vorticity equation. The linear term is $J(x,\nabla^2\chi)=p\pi Dd\sin X\sin Z$. The nonlinear cross term is

$$
J(\chi,\nabla^2\chi)=(p-4k^2)J(Dd\sin X\cos Z,Ee\sin2X).
$$

The Jacobian on the right is $2\pi kDEde\sin X\sin Z\cos2X$. Its retained component is $-\pi kDEde\sin X\sin Z$, so the total retained magnetic term is

$$
p\pi Dd[1+(3-\varphi)e]\sin X\sin Z.
$$

Meanwhile the projected acceleration, viscous term and temperature forcing have coefficients $-p^2S\dot a$, $p^2Sa$, and $-RkTb$. Divide the projected vorticity equation by $-p^2S$ to obtain $\dot a=\sigma[-a+rb+\zeta qd\{(\varphi-3)e-1\}]$, using $r=k^2R/p^3$ and $q=\pi^2Q/p^2$. This derives the complete [five-mode vertical-field magnetoconvection](../../../../../five-mode-vertical-field-magnetoconvection.md) system:

$$
\begin{aligned}
\dot a&=\sigma[-a+rb+\zeta qd\{(\varphi-3)e-1\}],\\
\dot b&=-b+a(1-c),&\dot c&=\varphi(-c+ab),\\
\dot d&=-\zeta d+a(1-e),&\dot e&=-(4-\varphi)\zeta e+\varphi ad.
\end{aligned}
$$

The [Rayleigh number](../../../../../rayleigh-number.md), [Chandrasekhar number](../../../../../chandrasekhar-number.md), [Prandtl number](../../../../../prandtl-number.md) and [magnetic-to-thermal diffusivity ratio](../../../../../magnetic-to-thermal-diffusivity-ratio.md) enter through r,q,$\sigma$ and $\zeta$ respectively.

Linearization at the zero-amplitude state leaves c and e with negative rates $-\varphi$ and $-(4-\varphi)\zeta$, while a,b,d have coefficient matrix

$$
L=\begin{pmatrix}-\sigma&\sigma r&-\sigma\zeta q\\1&-1&0\\1&0&-\zeta\end{pmatrix}.
$$

A zero eigenvector satisfies $b=a$, $d=a/\zeta$ and $[-1+r-q]a=0$. Thus **the stationary threshold is $\boxed{r_c=1+q}$**. The reversal symmetry $(a,b,c,d,e)\mapsto(-a,-b,c,-d,e)$ makes the nontrivial steady states occur as a pair.

For these nonzero steady states put $A=a^2$. The temperature equations give $c=ab$ and $b=a(1-c)$, so $b=a/(1+A)$ and $c=A/(1+A)$. The induction equations give $\zeta d=a(1-e)$ and $(4-\varphi)\zeta e=\varphi ad$. With $\mu=(4-\varphi)\zeta^2/\varphi$, their solution is

$$
\boxed{b=\frac a{1+a^2},\quad c=\frac{a^2}{1+a^2},\quad d=\frac{\mu a}{\zeta(\mu+a^2)},\quad e=\frac{a^2}{\mu+a^2}.}
$$

Here $k>0$ gives $0<\varphi<4$, and positive diffusivity gives $\mu>0$. Substituting these amplitudes into the stationary a equation and dividing by a yields the [stationary branch of five-mode magnetoconvection](../../../../../stationary-branch-of-five-mode-magnetoconvection.md):

$$
\boxed{r=1+a^2+\frac{q\mu(1+a^2)[\mu+(4-\varphi)a^2]}{(\mu+a^2)^2}.}
$$

At $a=0$ this meets $r=1+q$. Expansion in $A=a^2$ gives

$$
r=1+q+\left[1+q+\frac{q(2-\varphi)}\mu\right]A+O(A^2).
$$

The denominator of its initial slope is positive, and its numerator after multiplication by $(4-\varphi)\zeta^2$ is

$$
\mathcal N=(4-\varphi)\zeta^2(1+q)+\varphi q(2-\varphi).
$$

Therefore **$\mathcal N>0$ gives a [supercritical pitchfork bifurcation](../../../../../supercritical-pitchfork-bifurcation.md) direction, and $\mathcal N<0$ gives a [subcritical pitchfork bifurcation](../../../../../subcritical-pitchfork-bifurcation.md) direction.** If $\mathcal N=0$, the leading slope vanishes and higher terms must be retained.

This classification describes which side of the stationary threshold contains the steady branch. It does not alone establish dynamical stability or rule out an earlier oscillatory instability. For example, at $r_c$ the characteristic polynomial factors as

$$
\lambda\left[\lambda^2+(\sigma+1+\zeta)\lambda+\zeta(1+\sigma)+\sigma q(\zeta-1)\right].
$$

The zero eigenvalue is simple unless the final coefficient vanishes; the other two eigenvalues need not both be stable for every positive parameter choice. The stationary branch formula and its direction criterion remain the requested algebraic conclusions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
