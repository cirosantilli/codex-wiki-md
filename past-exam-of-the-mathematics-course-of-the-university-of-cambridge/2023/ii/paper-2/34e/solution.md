<h1 id="34e/solution">Solution</h1>

↑ **Parent:** [34E](../34e.md)

The spectral equation $(S)$ is

$$
-\phi_{xx}+u\phi=\lambda\phi,
\qquad\text{equivalently}\qquad
\phi_{xx}=(u-\lambda)\phi.
$$

This is the [KdV Schrodinger spectral problem](../../../../../kdv-schrodinger-spectral-problem.md). Differentiating it with respect to $t$ gives

$$
\phi_{xxt}=(u_t-\dot\lambda)\phi+(u-\lambda)\phi_t.
$$

For

$$
Q=\phi_t+u_x\phi-2(u+2\lambda)\phi_x,
$$

a direct differentiation, followed by substitution of the two preceding identities, yields

$$
Q_{xx}=(u-\lambda)Q+
\bigl(u_t+u_{xxx}-6uu_x-\dot\lambda\bigr)\phi.
$$

Therefore

$$
\begin{aligned}
\partial_x(\phi_xQ-\phi Q_x)
&=\phi_{xx}Q-\phi Q_{xx}\\
&=\phi^2\bigl(\dot\lambda-u_t-u_{xxx}+6uu_x\bigr).
\end{aligned}
$$

Comparison with $(*)$ gives

$$
\boxed{\alpha=-1.}
$$

This is the reusable [KdV Schrodinger spectral problem](../../../../../kdv-schrodinger-spectral-problem.md) [Wronskian identity](../../../../../wronskian.md).

Now take $u$ to satisfy the [Korteweg-De Vries equation](../../../../../korteweg-de-vries-equation.md) and $\phi=\varphi_n$, where $\lambda_n=-\kappa_n^2$. Both $\varphi_n$ and its derivative decay at infinity, as does $u$, so integration of $(*)$ over the real line gives

$$
0=\dot\lambda_n\int_{-\infty}^{\infty}\varphi_n^2\,dx
=\dot\lambda_n.
$$

The normalization was used in the last equality. Hence

$$
\boxed{\lambda_n(t)=\lambda_n(0)},
$$

which is the [Isospectrality of the KdV discrete spectrum](../../../../../isospectrality-of-the-kdv-discrete-spectrum.md).

With the KdV equation and $\dot\lambda_n=0$, the Wronskian identity says

$$
\partial_x(\varphi_{n,x}Q-\varphi_nQ_x)=0.
$$

Decay at infinity makes the constant zero. Thus $(Q/\varphi_n)_x=0$ between zeros, and continuation across the isolated zeros gives

$$
Q(x,t)=h_n(t)\varphi_n(x,t).
$$

Multiplying by $\varphi_n$ and integrating,

$$
h_n=\int\varphi_n\varphi_{n,t}\,dx
+\int u_x\varphi_n^2\,dx
-2\int(u+2\lambda_n)\varphi_n\varphi_{n,x}\,dx.
$$

The first integral is zero by differentiating the normalization. Integration by parts turns the last integral into $\int u_x\varphi_n^2dx$, so

$$
h_n=2\int u_x\varphi_n^2\,dx.
$$

To evaluate this, differentiate $(S)$ in $x$ and use it to write

$$
u_x\varphi_n^2
=\varphi_n\varphi_{n,xxx}-\varphi_{n,x}\varphi_{n,xx}.
$$

Its integral is $-2\int\varphi_{n,x}\varphi_{n,xx}dx=0$ by decay. Hence

$$
\boxed{h_n=0,\qquad Q=0.}
$$

As $x\to+\infty$, rapid decay of $u$ and $u_x$, together with

$$
\varphi_n\sim c_n(t)e^{-\kappa_nx},
\qquad
\varphi_{n,x}\sim-\kappa_nc_n(t)e^{-\kappa_nx},
$$

reduces $Q=0$ to

$$
c_n'-4\kappa_n^3c_n=0.
$$

Since $\kappa_n$ is constant,

$$
\boxed{c_n(t)=c_n(0)e^{4\kappa_n^3t},}
$$

as stated by the [Evolution of a KdV discrete norming constant](../../../../../evolution-of-a-kdv-discrete-norming-constant.md).

## ↑ Ancestors (10)

1. [34E](../34e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
