<h1 id="26h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The conclusion printed as convergence in probability is already an assumption; the substantive conclusion is convergence in $L^p$, and we prove that stronger statement.

First, the almost-sure subsequence result from part (a) and Fatou's lemma show that $X\in L^r$:

$$
\mathbb E|X|^r
\leq\liminf_k\mathbb E|X_{n_k}|^r<\infty.
$$

Consequently

$$
\sup_n\mathbb E|X_n-X|^r<\infty.
$$

Fix $1\leq p<r$ and $\delta>0$. Splitting according to  
$|X_n-X|\leq\delta$ and applying Hölder's inequality on the complement gives

$$
\begin{aligned}
\mathbb E|X_n-X|^p
&\leq\delta^p+
\mathbb E\!\left[|X_n-X|^p
1_{\{|X_n-X|>\delta\}}\right]\\
&\leq\delta^p+
\big(\mathbb E|X_n-X|^r\big)^{p/r}
\mathbb P(|X_n-X|>\delta)^{1-p/r}.
\end{aligned}
$$

The second term tends to zero because of convergence in probability and the uniform $L^r$ bound. Taking the upper limit and then $\delta\downarrow0$ proves

$$
\boxed{\|X_n-X\|_p\longrightarrow0}.
$$

This is [convergence in Lp from convergence in probability and an Lr bound](../../../../../../convergence-in-lp-from-convergence-in-probability-and-an-lr-bound.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26H](../../26h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
