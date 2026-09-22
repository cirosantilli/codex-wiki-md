<h1 id="7d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substituting

$$
y(z)=\int_\gamma e^{zt}f(t)\,dt,
\qquad y^{(3)}(z)=\int_\gamma e^{zt}t^3f(t)\,dt,
$$

and using $ze^{zt}=\partial_te^{zt}$ gives

$$
zy^{(3)}+2y
=[e^{zt}t^3f(t)]_{\partial\gamma}
+\int_\gamma e^{zt}\{2f(t)-(t^3f(t))'\}\,dt.
$$

It is therefore enough to require

$$
(t^3f)'=2f
$$

and choose $\gamma$ so that the [integral](../../../../../../integral.md) converges and $e^{zt}t^3f(t)$ vanishes at its endpoints. Solving the amplitude equation,

$$
\boxed{\frac{f'}f=\frac2{t^3}-\frac3t,
\qquad
f(t)=Ct^{-3}e^{-1/t^2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7D](../../7d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
