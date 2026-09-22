# Mixed Dirichlet-Neumann problem in an elliptic annulus

↑ **Parent:** [Elliptic coordinates](elliptic-coordinates.md)

In [elliptic coordinates](elliptic-coordinates.md) $x=\cosh\mu\cos\nu$, $y=\sinh\mu\sin\nu$, a [harmonic function](harmonic-function.md) in $a<\mu<b$, with $0<a<b$ and [period](period-of-a-function.md) $2\pi$ in $\nu$, satisfies $u_{\mu\mu}+u_{\nu\nu}=0$. Prescribe $u(b,\nu)=f(\nu)$ and $u_\mu(a,\nu)=g(\nu)$. Expand both boundary functions in [Fourier series](fourier-series-split.md), writing their constant terms as $f_0,g_0$. For either the [sine](sine.md) or [cosine](cosine.md) coefficient of order $n\geq1$, [separation of variables](separation-of-variables.md) gives

$$
u_n(\mu)=f_n\frac{\cosh[n(\mu-a)]}{\cosh[n(b-a)]}-g_n\frac{\sinh[n(b-\mu)]}{n\cosh[n(b-a)]}.
$$

The constant angular mode is $u_0(\mu)=f_0+g_0(\mu-b)$. These expressions follow by solving $u_n''-n^2u_n=0$ and checking $u_n(b)=f_n$, $u_n'(a)=g_n$. Their [Fourier series](fourier-series-split.md) gives the solution for sufficiently regular boundary data.

The phrase _normal derivative_ needs care: the [scale factor](scale-factor-cosmology.md) is $h=\sqrt{\sinh^2\mu+\sin^2\nu}$, so the outward [unit normal](unit-normal.md) derivative on the inner ellipse is $\partial_nu=-h^{-1}u_\mu$. Prescribing a physical [Neumann boundary condition](neumann-boundary-condition.md) therefore differs from prescribing $u_\mu$.

For [uniqueness](uniqueness.md), subtract two solutions to obtain $v$. Multiply $v_{\mu\mu}+v_{\nu\nu}=0$ by $v$ and use [integration by parts](integration-by-parts.md) over the periodic coordinate rectangle. The outer [Dirichlet boundary condition](dirichlet-boundary-condition.md), inner homogeneous derivative condition and periodic side cancellation give $\int_a^b\int_0^{2\pi}(v_\mu^2+v_\nu^2)\,d\nu\,d\mu=0$. Thus $v$ is constant, and the outer condition makes it zero.

## ↑ Ancestors (5)

1. [Elliptic coordinates](elliptic-coordinates.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/2/b/solution.md)
