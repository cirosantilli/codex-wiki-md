<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

Put $\delta=w-u$, which vanishes on the boundary. Expanding the [Dirichlet energy](../../../../../dirichlet-energy.md) gives

$$
\int_S|\nabla w|^2\,dA
=\int_S|\nabla u|^2\,dA+2\int_S\nabla u\cdot\nabla\delta\,dA+\int_S|\nabla\delta|^2\,dA.
$$

The cross term vanishes by integration by parts: it is $\int_{\partial S}\delta\partial_nu\,ds-\int_S\delta\Delta u\,dA=0$, using both the zero boundary values of $\delta$ and [Laplace's equation](../../../../../laplace-equation.md) for $u$. Thus the [Dirichlet principle](../../../../../dirichlet-principle.md) gives the stronger identity

$$
\boxed{\int_S|\nabla w|^2\,dA-\int_S|\nabla u|^2\,dA=\int_S|\nabla(w-u)|^2\,dA\geq0.}
$$

With the usual regular boundary, equality forces $w=u$.

In the unit disc, take boundary data $\cos\theta$. The [harmonic function](../../../../../harmonic-function.md) $u=r\cos\theta=x$ realizes these data and has constant [gradient](../../../../../gradient.md) of length one, so its energy is $\pi$. For $w=g(r)\cos\theta$, the polar [gradient](../../../../../gradient.md) gives

$$
\int_S|\nabla w|^2\,dA
=\int_0^1\int_0^{2\pi}\left[g'^2\cos^2\theta+\frac{g^2}{r^2}\sin^2\theta\right]r\,d\theta\,dr
=\pi\int_0^1\left(rg'^2+\frac{g^2}{r}\right)\,dr.
$$

The energy principle therefore yields the [sharp radial Dirichlet energy inequality](../../../../../sharp-radial-dirichlet-energy-inequality.md)

$$
\boxed{\int_0^1\left(rg'^2+\frac{g^2}{r}\right)dr\geq1.}
$$

There is a small regularity point at the centre: finite energy need not make the polar expression classically smooth there. The bound still holds under the stated finite-energy condition. Indeed for $0<s<t$,

$$
|g(t)^2-g(s)^2|
\leq2\left(\int_s^t rg'^2\,dr\right)^{1/2}
\left(\int_s^t\frac{g^2}{r}\,dr\right)^{1/2}.
$$

The tails tend to zero, so $g^2$ has a limit at zero. That limit must be zero, since a positive limit would make $\int g^2/r$ diverge. Completing the square on $[\varepsilon,1]$ and letting $\varepsilon\to0$ gives

$$
\int_0^1\left(rg'^2+\frac{g^2}{r}\right)dr
=1+\int_0^1r\left(g'-\frac gr\right)^2dr.
$$

This proves the finite-energy extension directly, and also shows that **equality holds exactly for $g(r)=r$**.

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
