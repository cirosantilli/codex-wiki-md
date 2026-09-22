# Robin diffusion with a growing mode

↑ **Parent:** [Diffusion equation](diffusion-equation-split.md)

These [Robin boundary conditions](robin-boundary-condition.md) give the spatial [Sturm-Liouville operator](sturm-liouville-operator.md) $-d^2/dx^2$ one negative [eigenvalue](eigenvalue.md), $-1$, with [eigenfunction](eigenfunction.md) $e^x$. The other eigenvalues are $n^2\pi^2$, with eigenfunctions $V_n=n\pi\cos(n\pi x)+\sin(n\pi x)$, $n\geq1$; there is no zero eigenvalue. Hence the [diffusion equation](diffusion-equation-split.md) has a growing contribution $c_0e^{t+x}$ in addition to decaying modes.

There is no contradiction with ordinary diffusive smoothing. The outward [normal derivative](normal-derivative.md) is $-u_x$ at the left endpoint and $u_x$ at the right endpoint, so imposing the same coordinate derivative at both ends does not impose dissipative outward-normal data at both ends. The energy identity is $\tfrac12\partial_t\int u^2=[uu_x]_0^1-\int u_x^2$, whose boundary term is $u(1)^2-u(0)^2$ here and can supply energy. Orthogonal projection of initial data $f$ gives $c_0=2\int_0^1fe^x\,dx/(e^2-1)$; it vanishes precisely when the growing mode is absent.

The reflected boundary conditions $u_x(0,t)=-u(0,t)$ and $u_x(1,t)=-u(1,t)$ have the same spectrum, because reflection $x\mapsto1-x$ reverses the coordinate derivative. Here the growing eigenfunction is $e^{-x}$ and the decaying functions are $W_n=n\pi\cos(n\pi x)-\sin(n\pi x)$, giving

$$
u(x,t)=c_0e^{t-x}+\sum_{n\geq1}c_ne^{-n^2\pi^2t}W_n(x).
$$

For square-integrable initial data $f$, [orthogonal projection](orthogonal-projection.md) gives

$$
c_0=\frac{2}{1-e^{-2}}\int_0^1e^{-x}f(x)dx,\qquad c_n=\frac{2}{n^2\pi^2+1}\int_0^1W_n(x)f(x)dx.
$$

The norms are $(1-e^{-2})/2$ and $(n^2\pi^2+1)/2$. The spatial [Sturm-Liouville problem](sturm-liouville-problem.md) has no zero eigenvalue and exactly one negative eigenvalue for $-D^2$, namely $-1$. The energy boundary term now reads $u(0)^2-u(1)^2$, so the left endpoint can supply energy. The growing mode disappears exactly when $\int_0^1e^{-x}f(x)dx=0$.

## ↑ Ancestors (6)

1. [Diffusion equation](diffusion-equation-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2/2/a/solution.md)
