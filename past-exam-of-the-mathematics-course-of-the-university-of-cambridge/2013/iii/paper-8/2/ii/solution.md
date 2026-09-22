<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [uniform bound for harmonic sine polynomials](../../../../../../uniform-bound-for-harmonic-sine-polynomials.md)

$$
P_m(t)=\sum_{k=1}^m\frac{\sin kt}{k},\qquad
\|P_m\|_\infty\leq C_0,\quad C_0=1+\pi.
$$

For completeness, reduce to $0<t\leq\pi$ and split at $K=\min(m,\lfloor1/t\rfloor)$. The first part is bounded by $Kt\leq1$. Geometric-series summation bounds every interval sum of $\sin kt$ by $1/\sin(t/2)\leq\pi/t$. [Summation by parts](../../../../../../abel-s-summation-formula.md) bounds the remaining harmonic-weighted tail by $\pi/[t(K+1)]\leq\pi$. Negative $t$ follows by oddness and $t=0$ is immediate.

Let $H_m=\sum_{k=1}^m1/k$. Choose $m_j$ so large that $H_{m_j}\geq C_0\,2^{j+2}$, and positive integers $L_j>m_j$ such that the intervals $[L_j-m_j,L_j+m_j]$ are strictly separated and increase. Define

$$
Q_j(t)=e^{iL_jt}\frac{P_{m_j}(t)}{H_{m_j}},\qquad
\boxed{g(t)=\frac12\sum_{j=1}^{\infty}Q_j(t).}
$$

The bound $\|Q_j\|_\infty\leq2^{-j-2}$ makes this a continuous function with $g(0)=0$.

Each [Fourier coefficient](../../../../../../fourier-coefficient.md) of $P_m$ has modulus $1/(2k)$, so the sum of the absolute coefficients is $H_m$. Therefore every prefix of a normalized block $Q_j$ has norm at most one. At any Fourier cutoff, all earlier blocks are complete, at most one block is partial and all later blocks are absent. Hence

$$
\boxed{\|S_ng\|_\infty
\leq\frac12\left(\sum_{j\geq1}2^{-j-2}+1\right)
=\frac58<1.}
$$

At zero, a completed block contributes zero, but its prefix through frequency $L_j$ consists of the negative-frequency sine coefficients and equals $i/2$. Thus

$$
S_{L_j}g(0)=\frac i4,\qquad
S_{L_j+m_j}g(0)=0.
$$

Both index sequences tend to infinity. **The uniformly bounded partial sums fail to converge at the origin**, even though the function is continuous and zero there.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
