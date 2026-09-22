<h1 id="11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

**Fourth-order spatial formula.** For a sufficiently smooth function, pair the [Taylor expansions](../../../../taylor-expansion.md) at opposite shifts:

$$
\begin{aligned}
u(x+h)+u(x-h)&=2u+h^2u''+\frac{h^4}{12}u^{(4)}+\frac{h^6}{360}u^{(6)}+O(h^8),\\
u(x+2h)+u(x-2h)&=2u+4h^2u''+\frac{4h^4}{3}u^{(4)}+\frac{8h^6}{45}u^{(6)}+O(h^8).
\end{aligned}
$$

Multiply the first sum by sixteen, subtract the second, and subtract $30u(x)$. The constant and fourth-derivative terms cancel, leaving

$$
-u(x+2h)+16u(x+h)-30u(x)+16u(x-h)-u(x-2h)=12h^2u''-\frac{2h^6}{15}u^{(6)}+O(h^8).
$$

Hence the [fourth-order centered second derivative](../../../../fourth-order-centered-second-derivative.md) satisfies

$$
\boxed{D_{4,h}u(x)=\frac{-u(x+2h)+16u(x+h)-30u(x)+16u(x-h)-u(x-2h)}{12h^2}=u''-\frac{h^4}{90}u^{(6)}+O(h^6).}
$$

Rearranging proves the requested $u''=D_{4,h}u+O(h^4)$, including its leading error coefficient.

**Explicit diffusion scheme.** Take $x_j=jh$, $h=1/N$, $t_n=n\tau$, and let $U_j^n$ approximate $\psi(x_j,t_n)$. Combining the [forward Euler method](../../../../euler-method.md) in time with $D_{4,h}$ in space gives

$$
\boxed{U_j^{n+1}=U_j^n+\frac{\tau}{12h^2}\left(-U_{j+2}^n+16U_{j+1}^n-30U_j^n+16U_{j-1}^n-U_{j-2}^n\right),\qquad U_j^0=f(jh).}
$$

To check the error, insert the exact solution. The [heat equation](../../../../heat-equation.md) gives $\psi_t=\psi_{xx}$, while the time [Taylor expansion](../../../../taylor-expansion.md) and the spatial formula give the one-step defect

$$
\psi(x_j,t_n+\tau)-\psi(x_j,t_n)-\tau D_{4,h}\psi(x_j,t_n)=\frac{\tau^2}{2}\psi_{tt}+\frac{\tau h^4}{90}\psi_{xxxxxx}+O(\tau^3+\tau h^6).
$$

Thus its unnormalized [local truncation error](../../../../local-truncation-error.md) is

$$
\boxed{O(\tau^2)+O(\tau h^4),}
$$

as requested. Dividing this defect by $\tau$ gives the normalized residual $O(\tau)+O(h^4)$; these are distinct error conventions.

**Boundary implementation.** The centered stencil requires two ghost values at each end. An [even-reflection closure for Neumann diffusion](../../../../even-reflection-closure-for-neumann-diffusion.md) imposes

$$
\boxed{U_{-1}^n=U_1^n,\quad U_{-2}^n=U_2^n,\quad U_{N+1}^n=U_{N-1}^n,\quad U_{N+2}^n=U_{N-2}^n.}
$$

The reflected first centered difference at either endpoint is zero. Apply the same evolution formula at the endpoints after substituting these ghost values; for example,

$$
U_0^{n+1}=U_0^n+\frac{\tau}{12h^2}(-2U_2^n+32U_1^n-30U_0^n).
$$

The ghost values also close the stencil at $j=1$ and $j=N-1$. They are determined auxiliary values, not new physical data. For a smooth solution compatible with the [Neumann boundary conditions](../../../../neumann-boundary-condition.md), differentiating those conditions in time and using the [heat equation](../../../../heat-equation.md) gives $\psi_{xxx}=\psi_{xxxxx}=\cdots=0$ at the endpoints. Thus even reflection preserves the smoothness needed for fourth-order spatial accuracy. If the initial data fail the required higher compatibility conditions, a uniform smooth error expansion through $t=0$ cannot be assumed.

For completeness, the reflected spatial operator has cosine [eigenvectors](../../../../eigenvector.md) $\cos(\ell\pi j/N)$ and [eigenvalues](../../../../eigenvalue.md)

$$
\lambda_\ell=-\frac4{h^2}\sin^2\frac{\ell\pi}{2N}\left(1+\frac13\sin^2\frac{\ell\pi}{2N}\right).
$$

The most negative one is $-16/(3h^2)$. Requiring $|1+\tau\lambda_\ell|\leq1$ gives the [forward Euler method](../../../../euler-method.md) stability restriction $\boxed{\tau/h^2\leq3/8}$ in the natural trapezoid-weighted discrete norm. A fourth-order spatial stencil does not remove the explicit diffusion time-step restriction.

**Implicit alternative.** The [Crank-Nicolson diffusion scheme](../../../../crank-nicolson-diffusion-scheme.md) using the same spatial operator and boundary closure is

$$
\boxed{\left(I-\tfrac\tau2D_{4,h}\right)U^{n+1}=\left(I+\tfrac\tau2D_{4,h}\right)U^n.}
$$

It has second-order time accuracy and fourth-order spatial accuracy for smooth compatible solutions; its one-step defect is $O(\tau^3)+O(\tau h^4)$. Each spatial [eigenvalue](../../../../eigenvalue.md) $\lambda\leq0$ has amplification factor $(1+\tau\lambda/2)/(1-\tau\lambda/2)$ of magnitude at most one, so it removes the explicit restriction for this boundary closure.

The price is solving a banded linear system at every step; the same matrix factorization can be reused for fixed $h$ and $\tau$. Large time steps still reduce accuracy. Moreover, the amplification factor tends to $-1$ as $\tau|\lambda|\to\infty$, so short spatial wavelengths can alternate sign with little numerical damping. Thus unconditional linear stability does not guarantee a monotone or well-resolved transient. Boundary accuracy and initial compatibility remain necessary with either time discretization.

## ↑ Ancestors (12)

1. [11](../11.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
