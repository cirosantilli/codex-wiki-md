<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $V_t=\langle X\rangle_t$ for the [quadratic variation](../../../../../../quadratic-variation.md) and set

$$
C(p,q)=\frac{pq-\sqrt{pq}}{q-1}
=\frac{\sqrt{pq}(\sqrt{pq}-1)}{q-1}.
$$

The [Hölder factorization of stochastic exponentials](../../../../../../holder-factorization-of-stochastic-exponentials.md) follows by adding exponents:

$$
\begin{aligned}
\frac1q\left(\sqrt{pq}X_t-\frac{pq}{2}V_t\right)
+\frac{q-1}{q}C(p,q)X_t
&=\frac{\sqrt{pq}+pq-\sqrt{pq}}qX_t-\frac p2V_t\\
&=pX_t-\frac p2V_t.
\end{aligned}
$$

Thus

$$
\boxed{\mathcal E(X)_t^p
=\mathcal E(\sqrt{pq}X)_t^{1/q}
\bigl(e^{C(p,q)X_t}\bigr)^{(q-1)/q}.}
$$

The subtraction inside the numerator is $\sqrt{pq}-1$, outside the square root.

The [stochastic exponential](../../../../../../doleans-dade-exponential.md) $\mathcal E(\sqrt{pq}X)$ starts at one and is a [nonnegative local martingale](../../../../../../nonnegative-local-martingale.md), hence a [supermartingale](../../../../../../supermartingale.md). The [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives expectation at most one at bounded stopping times. For a finite, possibly unbounded, stopping time $T$, apply this to $T\wedge n$, then use continuity and the [Fatou lemma](../../../../../../fatou-s-lemma.md):

$$
\mathbb E\mathcal E(\sqrt{pq}X)_T\leq1.
$$

The [Holder inequality](../../../../../../holder-inequality.md) with exponents $q$ and $q/(q-1)$ now gives

$$
\boxed{
\mathbb E[\mathcal E(X)_T^p]
\leq
\bigl(\mathbb E[e^{C(p,q)X_T}]\bigr)^{(q-1)/q}.}
$$

The inequality also holds when the right side is infinite.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
