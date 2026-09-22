<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the spatial spacing be $d$, the time step $k$, and $\mu=k/d$. Abbreviate the three new-time coefficients by $a=\mu(1+\mu)/2$, $b=(1+\mu)(2-\mu)$, $c=(1-\mu)(2-\mu)/2$, and the two old-time coefficients by $d_0=2-\mu$, $e_0=1+\mu$. These are the coefficients of the [compact third-order advection stencil](../../../../../../compact-third-order-advection-stencil.md).

For a smooth solution of the [advection equation](../../../../../../transport-equation.md), $u_t=u_x$ implies $u(x,t+k)=u(x+k,t)$. Substituting the exact solution into the stencil therefore evaluates all five terms on the same characteristic profile, at spatial offsets $(\mu-1)d$, $\mu d$, $(\mu+1)d$, $0$, and $d$. Its Taylor moments are

$$
M_j=a(\mu-1)^j+b\mu^j+c(\mu+1)^j-d_0\mathbf1_{\{j=0\}}-e_0.
$$

Direct polynomial expansion gives

$$
M_0=M_1=M_2=M_3=0,\qquad M_4=\mu(\mu+1)(\mu-1)(\mu-2)=K(\mu).
$$

Consequently the unscaled [local truncation error](../../../../../../local-truncation-error.md) is

$$
E=\frac{d^4}{24}K(\mu)u_{xxxx}+O(d^5).
$$

At a fixed nonzero [Courant number](../../../../../../courant-number.md), dividing by the time step gives an $O(d^3)$ consistency defect. Thus

$$
\boxed{\text{The stencil has order three for generic fixed }\mu.}
$$

When $K(\mu)=0$, the order is higher because the method simplifies to an exact integer shift: at $\mu=1$ the two sides have the common factor $2+e^{-i\theta}$ and the amplification is $e^{i\theta}$; at $\mu=2$ it is $e^{2i\theta}$. The signed value $\mu=-1$ gives the shift $e^{-i\theta}$, and $\mu=0$ gives the identity. These special cases do not invalidate the third-order statement for the family. Under the stability conditions established next, the usual accumulation of the fourth-order local defect over $O(1/k)$ steps gives third-order convergence for smooth data.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
