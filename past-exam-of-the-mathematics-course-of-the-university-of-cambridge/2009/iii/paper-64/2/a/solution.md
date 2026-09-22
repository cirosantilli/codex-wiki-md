<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [isothermal equation of state](../../../../../../globally-isothermal-equation-of-state.md), $p=c_s^2\rho$, with constant [isothermal sound speed](../../../../../../isothermal-sound-speed.md) $c_s$. A nonzero steady plane-parallel flow has constant mass flux $\rho u=j$. Choose the positive flow direction for convenience. The [continuity equation](../../../../../../continuity-equation.md) then gives $\rho'/\rho=-u'/u$, and the steady [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) becomes

$$
uu'=-c_s^2\frac{\rho'}{\rho}-\Phi'\quad\Longrightarrow\quad\left(u-\frac{c_s^2}{u}\right)u'=-\Phi'.
$$

Integrating and absorbing the reference [velocity](../../../../../../velocity.md) into the constant yields, for the [Mach number](../../../../../../mach-number.md) $\mathcal M=u/c_s$,

$$
\boxed{\tfrac12\mathcal M^2-\ln\mathcal M+\Phi/c_s^2=C.}
$$

For the opposite flow direction use $\mathcal M=|u|/c_s$; the same relation holds.

A smooth [sonic point](../../../../../../sonic-point.md) has $u=c_s$, so its momentum equation requires $\Phi'=0$. Moreover $f(\mathcal M)=\mathcal M^2/2-\ln\mathcal M$ satisfies $f'(1)=0$, $f''(1)=2$ and has its minimum $f(1)=1/2$. Thus, if the flow reaches $\mathcal M=1$ at $x_*$,

$$
f(\mathcal M)-\tfrac12=\frac{\Phi(x_*)-\Phi(x)}{c_s^2}\geq0.
$$

A sonic crossing is therefore possible at a maximum of the potential, with

$$
\boxed{C=\tfrac12+\Phi_{\max}/c_s^2.}
$$

At a nondegenerate maximum, the expansions give $(\mathcal M-1)^2=-\Phi''(x_*)(x-x_*)^2/(2c_s^2)+\cdots$. Choosing either smooth sign gives a crossing slope $\mathcal M'(x_*)=\pm\sqrt{-\Phi''(x_*)/(2c_s^2)}$, joining a [subsonic flow](../../../../../../subsonic-flow.md) to a [supersonic flow](../../../../../../supersonic-flow.md), or the reverse. This establishes the [plane-parallel isothermal sonic transition at a potential maximum](../../../../../../plane-parallel-isothermal-sonic-transition-at-a-potential-maximum.md). For a globally defined crossing, the same maximum must also be high enough for the Bernoulli relation to remain real over the intended domain.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
