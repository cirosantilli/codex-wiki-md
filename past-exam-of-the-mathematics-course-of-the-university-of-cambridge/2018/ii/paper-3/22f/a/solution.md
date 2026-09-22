<h1 id="22f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $1\leq p<\infty$, the [Lebesgue space](../../../../../../lp-space.md) $L^p(X)$ consists of equivalence classes modulo equality almost everywhere of measurable functions satisfying

$$
\lVert f\rVert_p
=\left(\int_X|f|^p\,d\mu\right)^{1/p}<\infty.
$$

The space $L^\infty(X)$ consists of essentially bounded measurable functions modulo equality almost everywhere, with norm

$$
\lVert f\rVert_\infty=\operatorname*{ess\,sup}_{x\in X}|f(x)|.
$$

Let $1\leq p<q<\infty$ and put $r=q/p>1$. By [Hölder's inequality](../../../../../../holder-inequality.md),

$$
\int_X|f|^p
\leq
\left(\int_X|f|^{pr}\right)^{1/r}
\mu(X)^{1-1/r}.
$$

Taking $p$th roots gives

$$
\boxed{\lVert f\rVert_p
\leq\mu(X)^{1/p-1/q}\lVert f\rVert_q.}
$$

For $q=\infty$, directly integrating $|f|^p\leq\lVert f\rVert_\infty^p$ gives the same endpoint estimate. Hence $L^q(X)\subseteq L^p(X)$ when $\mu(X)<\infty$, as in [Lp inclusion on a finite measure space](../../../../../../lp-inclusion-on-a-finite-measure-space.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22F](../../22f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
