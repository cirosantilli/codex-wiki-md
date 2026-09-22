# Catenary minimizes the integral of height along a fixed-length curve

↑ **Parent:** [Catenary](catenary.md)

Among [curves](curve.md) of fixed [arc length](arc-length.md) $L>2a$ joining $(-a,0)$ to $(a,0)$, the hanging [catenary](catenary.md) globally minimizes $\int y\,ds$. Parametrize a competitor by [arc length](arc-length.md) $s\in[-L/2,L/2]$, so $x'^2+y'^2=1$. [Integration by parts](integration-by-parts.md) and the fixed horizontal endpoint separation give, for every $b>0$,

$$
\int_{-L/2}^{L/2}y\,ds=-\int_{-L/2}^{L/2}sy'\,ds
=2ab-\int_{-L/2}^{L/2}(bx'+sy')\,ds
\geq2ab-\int_{-L/2}^{L/2}\sqrt{b^2+s^2}\,ds.
$$

The inequality is the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Equality requires $x'=b/\sqrt{b^2+s^2}$ and $y'=s/\sqrt{b^2+s^2}$. [Integration](integral-split.md) gives the [catenary](catenary.md)

$$
y=b\left[\cosh(x/b)-\cosh(a/b)\right],\qquad L=2b\sinh(a/b).
$$

The last equation has a unique positive $b$, since $\sinh q/q$ increases strictly for $q>0$. The equality [curve](curve.md) is a single-valued graph below the chord, so the same global bound proves the result under those additional restrictions.

## ↑ Ancestors (6)

1. [Catenary](catenary.md)
2. [Euler-Lagrange equation](euler-lagrange-equation.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/9/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/5/solution.md)
