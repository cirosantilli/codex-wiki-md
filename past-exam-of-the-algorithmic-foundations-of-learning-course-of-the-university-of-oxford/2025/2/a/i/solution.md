<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work for an arbitrary realization of the sequence, and set $u_t=X_t^TV_{t-1}^{-1}X_t$. In the [Loewner order](../../../../../loewner-order.md),

$$
V_{t-1}=\lambda I+\sum_{s<t}X_sX_s^T\succeq\lambda I.
$$

By the [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md), every [eigenvalue](../../../../../eigenvalue.md) of $V_{t-1}$ is at least $\lambda$. The [matrix inverse](../../../../../matrix-inverse-split.md) therefore has eigenvalues at most $\lambda^{-1}$, and

$$
0\leq u_t\leq\frac{\|X_t\|_2^2}{\lambda}\leq1.
$$

For $0\leq u\leq1$, put $g(u)=2\log(1+u)-u$. Since $g(0)=0$ and $g'(u)=(1-u)/(1+u)\geq0$, we have $u\leq2\log(1+u)$. The [matrix determinant lemma](../../../../../matrix-determinant-lemma.md) now gives

$$
\det V_t=\det V_{t-1}(1+u_t).
$$

Taking [logarithms](../../../../../logarithm.md) and using a [telescoping sum](../../../../../telescoping-sum.md),

$$
\boxed{\sum_{t=1}^n|X_t|_{V_{t-1}^{-1}}^2
=\sum_{t=1}^n u_t
\leq2\sum_{t=1}^n\log(1+u_t)
=2\log\frac{\det V_n}{\det V_0}.}
$$

This [elliptical potential bound](../../../../../elliptical-potential-bound.md) holds for every realization and every $n$, without a probabilistic exceptional event. The condition $\lambda\geq1$ is what ensures $u_t\leq1$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../../split.md)
6. [Algorithmic foundations of learning course of the University of Oxford](../../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
