<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Formal self-adjointness gives symmetry of $B$, and strict positivity gives positive definiteness, so $B$ is an [inner product](../../../../../../../inner-product.md). Bounded coefficients give $B[u,u]\leq C\|u\|_{H^1}^2$. To prove the lower bound, uniform ellipticity gives

$$
B[u,u]\geq\theta\|Du\|_2^2-\|c_-\|_\infty\|u\|_2^2.
$$

If no lower bound by the $H^1$ norm existed, choose $u_j\in H_0^1$ with $\|u_j\|_{H^1}=1$ and $B[u_j,u_j]\to0$. By [weak convergence in a Hilbert space](../../../../../../../weak-convergence-in-a-hilbert-space.md) and the [Rellich-Kondrachov compactness theorem](../../../../../../../rellich-kondrachov-theorem.md), a subsequence has $u_j\rightharpoonup u$ in $H_0^1$ and $u_j\to u$ in $L^2$. The principal energy has [weak lower semicontinuity](../../../../../../../weak-lower-semicontinuity.md): it is the squared $L^2$ norm of the bounded multiplication operator $a^{1/2}Du$. The potential term converges because $c$ is bounded. Hence

$$
B[u,u]\leq\liminf_jB[u_j,u_j]=0.
$$

Strict positivity forces $u=0$. The preceding ellipticity estimate now gives $\|Du_j\|_2\to0$, while $\|u_j\|_2\to0$, contradicting $\|u_j\|_{H^1}=1$. Thus [strict positivity implies coercivity for an elliptic Dirichlet form](../../../../../../../strict-positivity-implies-coercivity-for-an-elliptic-dirichlet-form.md), and

$$
\boxed{\alpha\|u\|_{H^1}^2\leq B[u,u]\leq C\|u\|_{H^1}^2.}
$$

The new norm is equivalent to the original norm, so the space remains complete.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
