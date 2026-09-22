<h1 id="differential-equations/9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Under the usual existence and boundary hypotheses for the [Laplace transform](../../../../laplace-transform.md),

$$
\boxed{\overline{f'}(p)=p\bar f(p)-f(0+),\qquad\overline{tf}(p)=-\frac d{dp}\bar f(p).}
$$

The first formula requires a finite right limit and sufficient regularity for [integration by parts](../../../../integration-by-parts.md); it is not to be applied blindly to the singular function $t^{-1/2}$. For that function and real $p>0$, substitute $s=\sqrt{pt}$:

$$
\int_0^\infty e^{-pt}t^{-1/2}dt=\frac2{\sqrt p}\int_0^\infty e^{-s^2}ds=\sqrt{\pi/p}.
$$

Use the second transform identity to obtain

$$
\boxed{\mathcal L\{\sqrt t\}(p)=\frac{\sqrt\pi}{2p^{3/2}}.}
$$

Take the time transform of the [heat equation](../../../../heat-equation.md), with [differentiation](../../../../differentiation.md) and boundary limits interpreted in the standard decaying heat-solution class. The initial value is zero, so $v_{xx}=p v-u(x,0)=pv$. Transforming the constant flux gives $v_x(0,p)=-1/p$. Decay selects the decreasing solution of the transformed [ordinary differential equation](../../../../ordinary-differential-equation.md), giving

$$
v(x,p)=B(p)e^{-\sqrt p\,x},\qquad-\sqrt p\,B(p)=-1/p.
$$

Consequently

$$
\boxed{v(x,p)=p^{-3/2}e^{-x\sqrt p},\qquad u(0,t)=2\sqrt{t/\pi}.}
$$

The boundary value follows by comparing $v(0,p)=p^{-3/2}$ with the transform of $\sqrt t$.

One can also check the decay and transform steps without relying on a merely pointwise limit under an [improper integral](../../../../improper-integral.md). Using the [complementary error function](../../../../complementary-error-function.md), the classical [heat](../../../../heat-equation.md) solution is

$$
u(x,t)=2\sqrt{t/\pi}\,e^{-x^2/(4t)}-x\,\operatorname{erfc}\left(\frac{x}{2\sqrt t}\right)=\int_x^\infty\operatorname{erfc}\left(\frac{s}{2\sqrt t}\right)ds.
$$

[Differentiation](../../../../differentiation.md) verifies $u_{xx}=u_t$, $u_x(0,t)=-1$, and $u(x,0)=0$ for $x>0$. Its integral representation gives $0\le u(x,t)\le2\sqrt{t/\pi}$ and pointwise decay as $x\to\infty$. Thus $e^{-pt}2\sqrt{t/\pi}$ supplies an integrable majorant, proving $v(x,p)\to0$ by [dominated convergence](../../../../dominated-convergence-theorem.md). The same representation gives the required regularity for the transforms. This explicitly verifies that the solution selected by the decaying transformed equation lies in the intended heat-solution class.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Differential equations](../../differential-equations.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
