<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The statement as printed is false without an integrability condition.** On any nonempty open set, the constant functions $f_n\equiv n$ are harmonic and therefore subharmonic, but their supremum is $+\infty$, which is not locally integrable.

A valid version assumes $g=\sup_n f_n\in L^1_{\rm loc}(\Omega)$. First, the maximum of finitely many subharmonic functions is subharmonic. For a distributional proof, mollify two functions on smaller interior domains and replace their maximum by

$$
M_\delta(s,t)=\frac12\left(s+t+\sqrt{(s-t)^2+\delta^2}\right).
$$

This is smooth, convex, and nondecreasing in each argument. The [chain rule](../../../../../../chain-rule.md) shows that its Laplacian applied to two smooth subharmonic functions is nonnegative: the first-derivative terms multiply their nonnegative Laplacians, and the Hessian term is nonnegative by convexity. [Mollifier](../../../../../../mollifier.md) convergence in $L^1_{\rm loc}$ and the uniform bound $|M_\delta-\max|\leq\delta/2$ allow both regularizations to be removed. Continuity of [distributional derivatives](../../../../../../distributional-derivative.md) under this convergence proves the finite-maximum assertion.

Now $g_N=\max_{n\leq N}f_n$ increases to $g$ and satisfies $|g_N|\leq|f_1|+|g|$ almost everywhere. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives convergence in $L^1_{\rm loc}$. For every nonnegative test function,

$$
\int g\,\Delta\varphi=\lim_{N\to\infty}\int g_N\,\Delta\varphi\geq0.
$$

Thus $g$ is subharmonic in the distributional sense. This is the [locally integrable supremum theorem for subharmonic functions](../../../../../../locally-integrable-supremum-theorem-for-subharmonic-functions.md). For the pointwise upper semicontinuous convention, take its canonical representative; the raw supremum need not already have that regularity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
