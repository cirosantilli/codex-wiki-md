# Fourth-order two-step advection stencil

↑ **Parent:** [Finite difference method](finite-difference-method.md)

For $u_t=u_x$, the recurrence $U_m^{n+1}-U_m^{n-1}=\sum_{j=\pm1,\pm2}a_jU_{m+j}^n$ has fourth-order normalized [consistency of a numerical method](consistency-of-a-numerical-method.md) at fixed $\mu=k/h$ if

$$
a_1=\mu(4-\mu^2)/3,\quad a_2=\mu(\mu^2-1)/6,\quad a_{-j}=-a_j.
$$

To derive this, match moments $M_r=\sum_ja_jj^r$ to the temporal [Taylor series](taylor-series.md): $M_0=M_2=M_4=0$, $M_1=2\mu$, $M_3=2\mu^3$. The even conditions force antisymmetry; the two odd conditions then determine the displayed coefficients. The normalized residual begins with $h^4(\mu^2-1)(\mu^2-4)u_{xxxxx}/120$. Its [amplification polynomial of a multilevel finite difference scheme](amplification-polynomial-of-a-multilevel-finite-difference-scheme.md) is $G^2-2iA(\theta)G-1$, where $A=a_1\sin\theta+a_2\sin2\theta$. At $\mu=1/2$, $|A|\le3/4$, giving a uniform power bound. At $\mu=3/2$, $A(\pi/3)=19\sqrt3/32>1$, and [wave packets](wave-packet.md) on the growing [polynomial root](root-of-a-polynomial.md) prove Cauchy [linear instability](linear-instability.md).

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/5/a/solution.md)
