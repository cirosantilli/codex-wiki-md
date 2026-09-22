<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $h=\Delta x$, $k=\Delta t$ and **$\mu=k/h$**, consistent with $u_t=u_x$ and the exact transport $u(x,t)=F(x+t)$. The PDF's middle implicit value is $u_m^{n+1}$; the converted TeX incorrectly places it at $m+1$.

Write the new-level coefficients at offsets $-1,0,1$ as $a=\mu(1+\mu)/2$, $b=(1+\mu)(2-\mu)$ and $c=(1-\mu)(2-\mu)/2$, and the old-level coefficients as $d=2-\mu$, $e=1+\mu$. Their sums are $a+b+c=d+e=3$. To compute the [local truncation error](../../../../../../local-truncation-error.md), expand the exact values $F(x_m+t_n+h(\mu+j))$ at the new level and $F(x_m+t_n+jh)$ at the old level. Equivalently the residual symbol is

$$
\mathcal E(z)=(ae^{-z}+b+ce^z)e^{\mu z}-(d+ee^z).
$$

The coefficients through $z^3$ vanish, while

$$
\mathcal E(z)=\frac{\mu(\mu-2)(\mu-1)(\mu+1)}{24}z^4+O(z^5).
$$

For example, the first three moment identities are $\sum_j a_j(\mu+j)^r=e$ for $r=1,2,3$, where $a_{-1}=a,a_0=b,a_1=c$; the fourth-moment difference is $\mu(\mu-2)(\mu-1)(\mu+1)$. Thus the exact residual is

$$
\frac{\mu(\mu-2)(\mu-1)(\mu+1)}{24}h^4F^{(4)}(x_m+t_n)+O(h^5).
$$

Normalizing the equation by $3k$ gives

$$
\boxed{\tau=\frac{(\mu-2)(\mu-1)(\mu+1)}{72}h^3u_{xxxx}+O(h^4).}
$$

For fixed nonzero $\mu\notin\{-1,1,2\}$, **the method has order three**. Its one-step residual is fourth degree, but the differential-equation truncation error is third order because of division by the time step.

There are exact transport exceptions. At $\mu=-1$ the equation reduces to $u_m^{n+1}=u_{m-1}^n$. At $\mu=2$ it gives $u_m^{n+1}=u_{m+2}^n$. At $\mu=1$, the exact shift $u_m^{n+1}=u_{m+1}^n$ satisfies the implicit equation, whose symbol is invertible as shown below. These are exact for every grid profile, not merely fourth-order exceptions. At $\mu=0$ the equation is the zero-time-step identity. These properties are summarized by the [rational implicit advection stencil with exact shift exceptions](../../../../../../rational-implicit-advection-stencil-with-exact-shift-exceptions.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
