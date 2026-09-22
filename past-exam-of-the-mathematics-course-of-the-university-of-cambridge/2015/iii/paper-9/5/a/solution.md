<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier coefficients](../../../../../../fourier-coefficient.md)

$$
b_n(y)=\frac2\pi\int_0^\pi u(x,y)\sin(nx)\,dx,\qquad n\geq1.
$$

They are continuous for $0\leq y\leq1$ and bounded by $2\|u\|_\infty$. On compact subintervals of $0<y<1$, the equation is [uniformly elliptic](../../../../../../uniformly-elliptic-operator.md) with smooth coefficients. Local [elliptic regularity](../../../../../../elliptic-regularity.md) at the flat vertical sides with zero boundary values permits differentiation and [integration by parts](../../../../../../integration-by-parts.md) there. Thus

$$
y^2b_n''(y)=-\frac2\pi\int_0^\pi u_{xx}(x,y)\sin(nx)\,dx=n^2b_n(y).
$$

For completeness, this identity also follows in the distributional sense without assuming boundary derivatives initially. Integrate on $(\varepsilon,\pi-\varepsilon)$ against $\sin(nx)$ and a [test function](../../../../../../test-function.md) of $y$ with support away from zero and one. The [interior gradient estimate near a zero Dirichlet side](../../../../../../interior-gradient-estimate-near-a-zero-dirichlet-side.md) gives $|u_x|\leq C\varepsilon^{-1}\sup|u|$ on a nearby ball of radius comparable to $\varepsilon$; continuity and the zero side value make that supremum $o(1)$ uniformly over the support in $y$. Therefore the boundary products $u_x\sin(nx)$ and $u\cos(nx)$ tend to zero. Move the $y$ derivatives to the [test function](../../../../../../test-function.md) before taking $\varepsilon\downarrow0$. This proves the [ordinary differential equation](../../../../../../ordinary-differential-equation.md), which makes each $b_n$ smooth in $0<y<1$ and yields the same classical identity.

The [Cauchy-Euler differential equation](../../../../../../cauchy-euler-equation.md) has [indicial roots](../../../../../../indicial-root.md)

$$
p_n^\pm=\frac{1\pm\sqrt{1+4n^2}}2,\qquad b_n(y)=A_n y^{p_n^+}+B_n y^{p_n^-}.
$$

For $n\geq1$ the negative root is strictly negative. Boundedness as $y\downarrow0$ forces $B_n=0$. Continuity at $y=1$ identifies

$$
A_n=\frac2\pi\int_0^\pi u(x,1)\sin(nx)\,dx,\qquad |A_n|\leq2\|u\|_\infty.
$$

Because $p_n^+>n$, the series $\sum_{n\geq1}A_ny^{p_n^+}\sin(nx)$ converges absolutely and uniformly for $0\leq y\leq\rho<1$. On compact subsets with $y>0$, differentiated series converge as well. At each fixed $0<y<1$, its [Fourier coefficients](../../../../../../fourier-coefficient.md) equal those of $u(\cdot,y)$; completeness of the [Fourier sine basis](../../../../../../fourier-sine-basis.md) in $L^2(0,\pi)$ and continuity in $x$ make the two functions equal. Therefore

$$
\boxed{u(x,y)=\sum_{n=1}^\infty A_ny^{(1+\sqrt{1+4n^2})/2}\sin(nx),\qquad (x,y)\in R.}
$$

This is also the requested sum over integers: take all coefficients with $n\leq0$ to be zero. Negative indices give redundant [Fourier modes](../../../../../../fourier-mode.md), and the $n=0$ sine vanishes. No pointwise convergence of the ordinary [Fourier series](../../../../../../fourier-series-split.md) on the top boundary is needed.

An important consequence is a [forced zero trace at a quadratically degenerate boundary](../../../../../../forced-zero-trace-at-a-quadratically-degenerate-boundary.md). Indeed the absolute sum is bounded by $2\|u\|_\infty\sum_{n\geq1}y^n=2\|u\|_\infty y/(1-y)$ for $y<1$, which tends to zero as $y\downarrow0$, uniformly in $x$. Thus **$u(x,0)=0$** on the entire lower side. It follows also from $b_n(0)=0$ for every sine coefficient and completeness.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
