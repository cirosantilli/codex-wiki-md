<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

By [weakly convergent sequence is bounded](../../../../../weakly-convergent-sequence-is-bounded.md), $M=\sup_n\|x_n\|^2$ is finite. Choose any $n_1$. Once $n_1<\cdots<n_k$ have been chosen, put $s_k=\sum_{j=1}^kx_{n_j}$. Since $s_k$ is fixed, [weak convergence](../../../../../weak-convergence.md) to zero gives $\langle s_k,x_n\rangle\to0$. Choose $n_{k+1}>n_k$ with $|\langle s_k,x_{n_{k+1}}\rangle|\leq1$. This gives the required one-sided inequality as well.

The useful estimate is for the **squared** [norm](../../../../../norm.md). Indeed, $\|s_1\|^2\leq M$, and the [inner product](../../../../../inner-product-split.md) expansion gives

$$
\|s_{k+1}\|^2
=\|s_k\|^2+2\langle s_k,x_{n_{k+1}}\rangle+\|x_{n_{k+1}}\|^2
\leq\|s_k\|^2+2+M.
$$

By [mathematical induction](../../../../../mathematical-induction.md), $\|s_k\|^2\leq Mk+2(k-1)\leq(M+2)k$. Hence

$$
\boxed{\left\|\frac1m\sum_{k=1}^m x_{n_k}\right\|^2\leq\frac{M+2}{m}\longrightarrow0.}
$$

This proves [norm convergence](../../../../../norm-convergence.md) of the averages, the [weak Banach–Saks theorem in a Hilbert space](../../../../../weak-banach-saks-theorem-in-a-hilbert-space.md). The printed inequality omits the square on its left side. Our stronger estimate also proves that printed bound, since $\sqrt{(M+2)k}\leq(M+2)k$ for $k\geq1$, but the printed bound alone only bounds the averages and cannot imply their [norm convergence](../../../../../norm-convergence.md) to zero.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
