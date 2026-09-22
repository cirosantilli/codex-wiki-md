<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A B-spline $N_j$ is positive exactly in the interior of its support $(t_j,t_{j+k})$. If the [B-spline collocation matrix](../../../../../../b-spline-collocation-matrix.md) $A_{\mathbf x}$ is invertible, its [determinant](../../../../../../determinant.md) contains a nonzero permutation term. Hence there is a permutation $\pi$ such that

$$
N_{\pi(r)}(x_r)\gt0,
\qquad r=1,\ldots,n.
$$

If $x_i\leq t_i$, then every one of the first $i$ points satisfies $x_r\lt t_i$. Any support containing such a point must have left endpoint $t_j\lt x_r$, hence $j\lt i$. Only $i-1$ B-splines are available to match these $i$ rows, contradicting that $\pi$ is a permutation. Thus $x_i\gt t_i$. Similarly, if $x_i\geq t_{i+k}$, each of the last $n-i+1$ points can only be matched to an index $j\gt i$, but only $n-i$ such indices exist. Therefore $x_i\lt t_{i+k}$. We have proved

$$
\boxed{t_i\lt x_i\lt t_{i+k}},
\qquad
\boxed{N_i(x_i)\gt0}.
$$

The [Schoenberg–Whitney theorem](../../../../../../schoenberg-whitney-theorem.md) states, for strictly increasing knots and interpolation sites, that

$$
\boxed{A_{\mathbf x}=(N_j(x_i))_{i,j=1}^n
\text{ is invertible}
\iff t_i\lt x_i\lt t_{i+k}
\iff N_i(x_i)\gt0\quad\forall i}.
$$

Indeed its determinant is positive under these inequalities.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
