<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the positive [mass accretion rate](../../../../../../mass-accretion-rate.md) $\dot M=-\mathcal J$, and retain $\delta=\gamma-1$, $q=2/\beta-1/2$. Define $h=1-q\delta$, which is positive under the condition in (b). Matching the [Bernoulli function](../../../../../../bernoulli-function.md) to the reservoir and using the [polytropic equation of state](../../../../../../polytropic-equation-of-state.md) gives

$$
c_*^2=\frac{c_\infty^2}{h},\qquad
r_*=\left(\frac{A\beta h}{2c_\infty^2}\right)^{1/\beta},
\qquad
\rho_*=\rho_\infty h^{-1/\delta}.
$$

The [transonic spherical accretion rate in a power-law potential](../../../../../../transonic-spherical-accretion-rate-in-a-power-law-potential.md) is therefore

$$
\boxed{\dot M=
4\pi\rho_\infty
\left(\frac{A\beta}{2}\right)^{2/\beta}
c_\infty^{\,1-4/\beta}
h^{\,q-1/\delta}.}
$$

The combination $A/c_\infty^2$ has dimensions of length to the power $\beta$, so this expression has dimensions of mass per time. The [sonic point](../../../../../../sonic-point.md) selects the flux that connects the subsonic reservoir to the inward supersonic [transonic branch](../../../../../../transonic-branch.md).

For the [endpoint limits of power-law spherical accretion](../../../../../../endpoint-limits-of-power-law-spherical-accretion.md), hold $A,\beta,\rho_\infty,c_\infty$ fixed. As $\delta\to0$, $\ln h=-q\delta+O(\delta^2)$, so $(q-1/\delta)\ln h\to q$. Hence

$$
\boxed{\lim_{\gamma\to1}\dot M=
4\pi\rho_\infty
\left(\frac{A\beta}{2}\right)^{2/\beta}
c_\infty^{\,1-4/\beta}e^{\,2/\beta-1/2}.}
$$

This is also obtained directly from an [isothermal equation of state](../../../../../../globally-isothermal-equation-of-state.md): the [Bernoulli function](../../../../../../bernoulli-function.md) becomes $u^2/2+c_\infty^2\ln(\rho/\rho_\infty)-A/r^\beta=0$, so $\rho_*/\rho_\infty=e^q$. For $\beta=1$, $A=GM$, it recovers the [isothermal Bondi accretion rate](../../../../../../isothermal-bondi-accretion-rate.md).

For $0<\beta<4$, $q>0$ and $\gamma\uparrow f(\beta)$ means $h\downarrow0$. Since $\delta=(1-h)/q$,

$$
h^{q-1/\delta}
=\exp\left[-\frac{qh\ln h}{1-h}\right]\longrightarrow1.
$$

Thus

$$
\boxed{\lim_{\gamma\uparrow f(\beta)}\dot M=
4\pi\rho_\infty
\left(\frac{A\beta}{2}\right)^{2/\beta}
c_\infty^{\,1-4/\beta}.}
$$

The finite limiting flux accompanies $r_*\to0$ and $c_*,\rho_*\to\infty$; it does not assert a finite-radius [sonic point](../../../../../../sonic-point.md) at the endpoint. For $\beta=1$ this is the familiar $\gamma\uparrow5/3$ limit $\pi G^2M^2\rho_\infty/c_\infty^3$.

For completeness, the printed range $\beta\geq4$ has the endpoint $f=+\infty$. At $\beta=4$, $q=0$ and the flux is independent of $\gamma$, namely $4\pi\rho_\infty(2A)^{1/2}$. For $\beta>4$, $q<0$ and $h\sim |q|\delta$, so $\dot M\to0$ as $\gamma\to\infty$. These are the corresponding extended endpoint limits.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
