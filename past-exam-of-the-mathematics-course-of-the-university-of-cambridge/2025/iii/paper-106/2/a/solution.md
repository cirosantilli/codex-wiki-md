<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a norm-dense sequence $(f_n)$ in the unit sphere of the separable dual $X^*$. For every $n$, choose $x_n\in B_X$ with $|f_n(x_n)|>1/2$. If a functional $f\in X^*$ vanished on the closed linear span of the $x_n$, normalize it and choose $f_n$ with $\|f-f_n\|<1/4$; then $|f(x_n)|>1/4$, a contradiction. The [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) therefore shows that the span of $(x_n)$ is dense, so $X$ is separable.

Choose a norm-dense sequence $(u_n)$ in $B_X$. On $B_{X^*}$ define

$$
d_*(f,g)=\sum_{n=1}^\infty2^{-n}
\frac{|(f-g)(u_n)|}{1+|(f-g)(u_n)|}.
$$

Weak-star convergence implies convergence in this metric. Conversely, metric convergence gives convergence on the dense set $(u_n)$, and the uniform norm bound on the dual ball extends it to every $u\in X$. Thus $d_*$ metrizes the weak-star topology, proving [weak-star metrizability of the dual ball](../../../../../../weak-star-metrizability-of-the-dual-ball.md).

Similarly, for a norm-dense sequence $(f_n)$ in $B_{X^*}$,

$$
d(x,y)=\sum_{n=1}^\infty2^{-n}
\frac{|f_n(x-y)|}{1+|f_n(x-y)|}
$$

metrizes the weak topology on $B_X$. Indeed, convergence against the dense functionals extends to every $f\in X^*$ because $x-y$ remains norm bounded.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
