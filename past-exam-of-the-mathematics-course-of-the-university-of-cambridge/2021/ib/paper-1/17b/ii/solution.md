<h1 id="17b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $e_n=y^n-y(t_n)$. Subtracting the exact one-step relation from the numerical method and applying the stated [Lipschitz continuity](../../../../../../lipschitz-continuity.md) gives

$$
\|e_{n+1}\|
\leq(1+hL)\|e_n\|+\|\tau_{n+1}\|.
$$

If $\|\tau_{n+1}\|\leq Ch^{p+1}$, iteration yields the [discrete Gronwall inequality](../../../../../../discrete-gronwall-inequality.md)

$$
\|e_n\|
\leq(1+hL)^n\|e_0\|
+Ch^{p+1}\sum_{j=0}^{n-1}(1+hL)^j.
$$

For $nh\leq t^*$,

$$
(1+hL)^n\leq e^{nhL}\leq e^{t^*L}
$$

and

$$
h^{p+1}\sum_{j=0}^{n-1}(1+hL)^j
\leq\frac{e^{t^*L}-1}{L}h^p.
$$

Consequently

$$
\boxed{
\max_{0\leq n\leq\lfloor t^*/h\rfloor}
\|y^n-y(nh)\|
\leq e^{t^*L}\|e_0\|+O(h^p)}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [17B](../../17b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
