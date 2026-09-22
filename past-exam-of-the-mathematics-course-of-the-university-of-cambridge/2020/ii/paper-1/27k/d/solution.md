<h1 id="27k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix an integer $k>n$ and partition $[0,1]$, up to endpoints of measure zero, into

$$
I_p=[(p-1)/k,p/k),
\qquad 1\le p\le k.
$$

For $p\ne q$, define

$$
f_{p,q}=\sqrt{\frac{k}{2}}\,
(\mathbf1_{I_p}-\mathbf1_{I_q}).
$$

These functions have integral zero and $L^2$ norm one, so they are admissible.

Let

$$
N_p=\sum_{i=1}^n\mathbf1_{\{Z_i\in I_p\}}
$$

be the interval occupancy counts. Since each $Z_i$ is uniform, $\mathbb EN_p=n/k$, and hence

$$
D(f_{p,q})
=\frac{k}{2n^2}\mathbb E(N_p-N_q)^2.
$$

For every outcome,

$$
\begin{aligned}
\sum_{p,q=1}^k(N_p-N_q)^2
&=2k\sum_{p=1}^kN_p^2-2\left(\sum_{p=1}^kN_p\right)^2\\
&=2k\sum_{p=1}^kN_p^2-2n^2\\
&\ge2kn-2n^2,
\end{aligned}
$$

because the nonnegative integer counts satisfy $N_p^2\ge N_p$ and $\sum_pN_p=n$. No independence assumption was used.

Averaging over all ordered pairs gives

$$
\frac1{k^2}\sum_{p,q=1}^kD(f_{p,q})
\ge\frac1n-\frac1k.
$$

The diagonal terms vanish, so some admissible pair $p\ne q$ satisfies the same lower bound. Therefore

$$
\sup_{\substack{\|f\|_2=1\\\int f\,d\lambda=0}}D(f)
\ge\frac1n-\frac1k.
$$

Letting $k\to\infty$ proves the [dependent uniform sampling variance lower bound](../../../../../../dependent-uniform-sampling-variance-lower-bound.md)

$$
\boxed{\sup D(f)\ge\frac1n}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [27K](../../27k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
