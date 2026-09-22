<h1 id="29c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Fourier coefficients](../../../../../../fourier-coefficient.md) obey $\dot u_n+(1+n^2)u_n=f_n$, so

$$
\boxed{u(t,x)=\sum_{n\in\mathbb Z}\left[\frac{f_n}{1+n^2}+\left((u_0)_n-\frac{f_n}{1+n^2}\right)e^{-(1+n^2)t}\right]e^{inx}.}
$$

The coefficient decay of $u_0,f$ and the additional exponential damping justify all derivatives for $t>0$ and recovery of the initial data. Thus this is a smooth periodic solution. Every transient mode decays, giving $\boxed{u(t,\cdot)\to u_f}$ uniformly, indeed with all spatial derivatives. The elliptic solution in part (i) is the attracting steady state of this forced [heat equation](../../../../../../heat-equation.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [29C](../../29c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
