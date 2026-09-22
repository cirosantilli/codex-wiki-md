<h1 id="30e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $m_0=\min_xu(x,0)>0$, which exists by periodicity and continuity. Fix any finite interval $[0,T]$ on which the classical solution is smooth. Choose $\epsilon>0$ with $\epsilon(1+T)<m_0/2$ and consider the strictly positive decreasing barrier $b(t)=m_0-\epsilon(1+t)$.

Initially $u>b$. If this strict inequality first failed, compactness of the spatial circle would give a first contact $(x_*,t_*)$ with $u=b>0$. At that contact, the spatial minimum of $u-b$ has $u_x=0$, $u_{xx}\geq0$, and the first-contact condition gives $(u-b)_t\leq0$. But the equation yields

$$
(u-b)_t=u^2u_{xx}+u^3+\epsilon>0,
$$

a contradiction. Therefore $u>b$ throughout the interval. Letting $\epsilon\downarrow0$ gives **$\boxed{u(x,t)\geq m_0>0}$** on $[0,T]$. Since $T$ was arbitrary, positivity persists for every time for which the assumed smooth solution exists. This argument is a [parabolic comparison principle](../../../../../../parabolic-comparison-principle.md) proved directly and does not assume uniform parabolicity before positivity has been established.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30E](../../30e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
