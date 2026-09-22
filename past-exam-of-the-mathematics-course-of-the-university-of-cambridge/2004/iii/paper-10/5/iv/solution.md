<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $c=f(1)\geq0$. For a given $x$, let $M=\|x\|^2=\|xx^*\|$ by the [C-star identity](../../../../../../c-star-identity.md). For $\varepsilon>0$ the binomial series

$$
b_\varepsilon=\sqrt{M+\varepsilon}\left(1-\frac{xx^*}{M+\varepsilon}\right)^{1/2}
$$

converges absolutely in the [Banach algebra](../../../../../../banach-algebra-split.md), because $\|xx^*/(M+\varepsilon)\|<1$. Its coefficients are real and $xx^*$ is Hermitian, so $b_\varepsilon^*=b_\varepsilon$; multiplication of the absolutely convergent series gives $b_\varepsilon^*b_\varepsilon=(M+\varepsilon)1-xx^*$. Positivity yields $f(xx^*)\leq(M+\varepsilon)c$. Let $\varepsilon\downarrow0$. Part (iii) now gives

$$
|f(x)|^2\leq c^2\|x\|^2.
$$

Thus $f$ is a [bounded linear functional](../../../../../../continuous-linear-functional.md) with $\|f\|\leq c$. Since the nonzero identity in a [C-star algebra](../../../../../../c-star-algebra.md) has norm one, evaluating at it gives the reverse bound. Hence

$$
\boxed{\|f\|=f(1).}
$$

This proves automatic continuity from the original algebraic positivity assumption, including the case $c=0$, when $f=0$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
