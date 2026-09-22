<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Integrating the given expansion equation gives $R^{3/2}=t/t_0$, with the integration constant fixed by $R(t_0)=1$. Thus the [scale factor](../../../../../scale-factor-cosmology.md) and [Hubble parameter](../../../../../hubble-parameter.md) are $R=(t/t_0)^{2/3}$ and $H=2/(3t)$. The [Newtonian derivation of the flat Friedmann equation](../../../../../newtonian-derivation-of-the-flat-friedmann-equation.md) gives $H^2=8\pi G\rho/3$, so

$$
\rho=\frac1{6\pi Gt^2},\qquad c^2=\gamma K\rho^{\gamma-1}=c^2(t_0)(t/t_0)^{-2(\gamma-1)}.
$$

Use the [comoving coordinate](../../../../../comoving-coordinate.md) $\boldsymbol q=\boldsymbol x/R$ and the [density contrast](../../../../../density-contrast.md) $\delta=\rho_1/\rho$. Linearized [mass conservation](../../../../../mass-conservation.md), the peculiar-velocity [Euler equation for fluid motion](../../../../../euler-equations-for-an-inviscid-fluid.md) and the [Poisson equation](../../../../../poisson-equation.md) for the [peculiar gravitational potential](../../../../../peculiar-gravitational-potential.md) are

$$
\dot\delta=-R^{-1}\nabla_q\cdot\boldsymbol v,\qquad
\dot{\boldsymbol v}+H\boldsymbol v=-R^{-1}\nabla_q(c^2\delta+\Phi),\qquad
\nabla_q^2\Phi=4\pi GR^2\rho\delta.
$$

Differentiate the first equation, substitute the second and use the third. A Fourier component of comoving [wavenumber](../../../../../wavenumber.md) $k$ obeys

$$
\ddot\varepsilon+2H\dot\varepsilon+\left(\frac{c^2k^2}{R^2}-4\pi G\rho\right)\varepsilon=0.
$$

Since $c^2k^2/R^2=k^2c^2(t_0)t_0^{2\gamma-2/3}t^{-2\gamma+2/3}$, the normalization is $\Lambda=kc(t_0)t_0^{\gamma-1/3}$, as printed in the PDF. The resulting [linear cosmological density perturbation](../../../../../linear-cosmological-density-perturbation-split.md) equation is

$$
\boxed{\ddot\varepsilon+\frac4{3t}\dot\varepsilon+\left(\frac{\Lambda^2}{t^{2\gamma-2/3}}-\frac2{3t^2}\right)\varepsilon=0.}
$$

To reduce it to a [Bessel equation](../../../../../bessel-differential-equation.md), put $\nu=\gamma-4/3$, $z=\Lambda/(\nu t^\nu)$ and $\varepsilon=t^a y(z)$. As $\dot z=-\nu z/t$, multiplying the substituted equation by $t^{2-a}$ gives

$$
\nu^2z^2y''+\nu(\nu-2a-1/3)zy'+\left[\nu^2z^2+a^2+a/3-2/3\right]y=0.
$$

Taking $a=-1/6$ makes the first two coefficients proportional to those in the [Bessel equation](../../../../../bessel-differential-equation.md), and the remaining constant is $-25/36$. Hence

$$
\boxed{\nu=\gamma-\frac43\in(0,1/3),\qquad\lambda=\frac5{6\nu}=\frac5{6\gamma-8}.}
$$

For noninteger $\lambda$, the [Bessel density modes of a polytropic expanding universe](../../../../../bessel-density-modes-of-a-polytropic-expanding-universe.md) are

$$
\boxed{\varepsilon=t^{-1/6}\left[A J_{-\lambda}(z)+B J_\lambda(z)\right].}
$$

There is an exceptional case within the allowed interval: if $\lambda=n$ is an integer, $J_{-n}=(-1)^nJ_n$, so these are not two independent solutions. The full solution then uses $t^{-1/6}[A Y_n(z)+B J_n(z)]$, with the [Bessel function of the second kind](../../../../../bessel-function-of-the-second-kind.md) providing the missing branch. For example $\gamma=29/18$ gives $\lambda=3$. A basis using $J_\lambda,Y_\lambda$ is valid for every allowed exponent.

For early times, $z\to\infty$. The [large-argument asymptotic expansion of the Bessel function of the first kind](../../../../../large-argument-asymptotic-expansion-of-the-bessel-function-of-the-first-kind.md) has oscillatory phase $z-\pi a/2-\pi/4$ and envelope $(2/(\pi z))^{1/2}$ for order $a$; the [Bessel function of the second kind](../../../../../bessel-function-of-the-second-kind.md) has the same envelope. Thus

$$
|\varepsilon|_{\rm envelope}\propto t^{-1/6}z^{-1/2}\propto\boxed{t^{\nu/2-1/6}=t^{(3\gamma-5)/6}.}
$$

This decreases because $3\gamma<5$. At late times $z\to0$, the leading powers are $J_{\pm\lambda}(z)\propto z^{\pm\lambda}$ for noninteger order, giving $t^{-1}$ and $t^{2/3}$. The $Y_n$ branch gives the same growing power in the integer case. Therefore **a generic perturbation grows as $t^{2/3}$**; an initial condition with zero growing-mode coefficient instead has the decaying $t^{-1}$ mode.

To find the growth scale including its dependence on $\nu$, set $\varepsilon=t^{2/3}h(t)$. The equation becomes

$$
h''+\frac8{3t}h'+\Lambda^2t^{-2\nu-2}h=0.
$$

Substitute $h=1+a\Lambda^2t^{-2\nu}+\cdots$. The leading coefficient equation is $-2\nu(5/3-2\nu)a+1=0$. The [pressure correction to a growing polytropic cosmological mode](../../../../../pressure-correction-to-a-growing-polytropic-cosmological-mode.md) is consequently

$$
\varepsilon_+=C t^{2/3}\left[1+\frac{\Lambda^2t^{-2\nu}}{2\nu(5/3-2\nu)}+\cdots\right].
$$

Since $ck/R=\Lambda t^{-\nu-1}$ and $t^{-2}=6\pi G\rho$, the correction becomes small when $(ck/R)^2t^2$ is small compared with $2\nu(5/3-2\nu)$. The factor $2(5/3-2\nu)$ is between two and $10/3$, giving the stated order-of-magnitude onset condition

$$
\boxed{\frac{ck}{R}\lesssim\sqrt{6\pi\nu G\rho}.}
$$

For a well-developed asymptotic growing mode, replace $\lesssim$ by $\ll$. This is a [Jeans instability](../../../../../jeans-instability.md) interpretation: the physical acoustic frequency must be sufficiently low compared with the gravitational expansion scale, or equivalently the physical wavelength must be sufficiently long for self-gravity to overcome pressure support. It is an approximate condition for the dust-like growing branch, not an exact initial-condition-independent instant at which any perturbation begins increasing. The instantaneous sign change of the coefficient in the original equation instead occurs at $c^2k^2/R^2=4\pi G\rho$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
