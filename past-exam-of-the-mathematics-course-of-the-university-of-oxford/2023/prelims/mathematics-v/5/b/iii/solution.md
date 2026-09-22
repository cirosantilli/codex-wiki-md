<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the stated inward heating, take $Q\geq0$ and put $\tau=\pi^2kt/(16\ell^2)$. Since $|\cos(\mu_nx)|\leq1$, the transient from [ii](../ii.md) satisfies

$$
|T(x,t)-T_s(x)|\leq\frac{16Q\ell}{k\pi^2}
\sum_{n=0}^\infty\frac{e^{-(2n+1)^2\tau}}{(2n+1)^2}.
$$

Equality holds at $x=0$, where every cosine is one and all coefficients have the same sign. Thus the maximum is attained at the heated end, and its exact value and late-time form are

$$
\begin{aligned}
\max_{0\leq x\leq2\ell}|T(x,t)-T_s(x)|
&=\frac{16Q\ell}{k\pi^2}e^{-\tau}
\left(1+\frac19e^{-8\tau}+O(e^{-24\tau})\right)\\
&\sim\boxed{\frac{16}{\pi^2}\frac{Q\ell}{k}
\exp\!\left(-\frac{\pi^2}{16}\frac{kt}{\ell^2}\right)}.
\end{aligned}
$$

This is dominance of the slowest-decaying [eigenfunction](../../../../../../../eigenfunction.md) when $kt\gg\ell^2$. More explicitly, the omitted relative correction is nonnegative and bounded by $(\pi^2/8-1)e^{-8\tau}$, using $\sum_{n\geq0}(2n+1)^{-2}=\pi^2/8$. For a signed imposed [heat flux](../../../../../../../heat-flux-density.md), the maximum-deviation formula uses $|Q|$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
