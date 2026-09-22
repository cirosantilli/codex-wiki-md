<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove [fourth-moment tightness of polygonal random walks](../../../../../../fourth-moment-tightness-of-polygonal-random-walks.md) uniformly, including intervals shorter than a mesh cell or crossing a mesh boundary. For $s<t$, let $c_j$ be the length of the overlap of $(Ns,Nt)$ with $(j-1,j)$. The interpolated increment is

$$
S_t^N-S_s^N=N^{-1/2}\sum_jc_j\xi_j,
\qquad 0\le c_j\le1,\qquad \sum_jc_j=N(t-s).
$$

Put $m_4=\mathbb E\xi^4<\infty$. Expanding the fourth power and using centered [independent](../../../../../../independent-random-variables.md) steps, only the terms with four equal indices or two equal pairs survive. Consequently

$$
\mathbb E|S_t^N-S_s^N|^4
=N^{-2}\left(m_4\sum_jc_j^4+6\sum_{i<j}c_i^2c_j^2\right)
=N^{-2}\left(3\left(\sum_jc_j^2\right)^2+(m_4-3)\sum_jc_j^4\right).
$$

If $m_4\le3$, the last correction is nonpositive. If $m_4>3$, use $\sum c_j^4\le(\sum c_j^2)^2$. In either case the expression is at most $\max(3,m_4)N^{-2}(\sum c_j^2)^2$. Since $c_j^2\le c_j$,

$$
\boxed{\mathbb E|S_t^N-S_s^N|^4\le\max(3,m_4)|t-s|^2,\quad\text{for all }N,s,t.}
$$

Also $S_0^N=0$ and the paths are continuous. The stated tightness criterion applies with $\gamma=4$, $\alpha=1$ and the displayed constant, so the laws $\mu_N$ are tight on $C_0([0,1],\mathbb R)$ with its uniform topology. Part (a) established all the Brownian [finite-dimensional distribution](../../../../../../finite-dimensional-distribution.md) limits. The supplied implication from tightness plus those limits now yields the [Donsker invariance principle](../../../../../../donsker-s-theorem.md):

$$
\boxed{\mu_N\Rightarrow\mu\quad\text{in }C([0,1],\mathbb R),}
$$

where $\mu$ is [Wiener measure](../../../../../../wiener-measure.md). No estimate restricted to grid endpoints would suffice by itself for the printed uniform criterion; the overlap coefficients handle every pair of times.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
