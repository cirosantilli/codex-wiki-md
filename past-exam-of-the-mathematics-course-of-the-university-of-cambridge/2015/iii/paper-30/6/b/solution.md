<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the real Hilbert space $L^2(\mathbb R_+)$, let $f_t=1_{[0,t]}$. Then $k_i(t)=\langle f_t,h_i\rangle$. The [Parseval identity for a Hilbertian basis](../../../../../../parseval-identity-for-a-hilbertian-basis.md) gives

$$
\begin{aligned}
K(s,t)&=\sum_i\langle f_s,h_i\rangle\langle f_t,h_i\rangle\\
&=\langle f_s,f_t\rangle
=\int_0^\infty1_{[0,s]}(u)1_{[0,t]}(u)\,du
=\min(s,t).
\end{aligned}
$$

The series is absolutely convergent by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), since $\sum_i k_i(s)^2=s$ and $\sum_i k_i(t)^2=t$. Thus

$$
\boxed{K(s,t)=s\wedge t,}
$$

the [Brownian covariance kernel](../../../../../../brownian-covariance-kernel.md). This is the [Brownian covariance from an integrated orthonormal basis](../../../../../../brownian-covariance-from-an-integrated-orthonormal-basis.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
