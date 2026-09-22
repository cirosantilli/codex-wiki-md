<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p\in A$, $r=f-p$, $E=\|r\|_\infty$ and $M=\{x\in[0,1]:|r(x)|=E\}$. The [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md) says

$$
\boxed{p\text{ is best}\quad\Longleftrightarrow\quad\forall h\in A,\ \min_{x\in M}r(x)h(x)\le0.}
$$

If $E=0$, $p=f$ is already best and the criterion holds. Suppose $E>0$. If $q=p+h$ were strictly better, then $|r(x)-h(x)|<|r(x)|=E$ on $M$, which forces $r(x)h(x)>0$ there. Conversely, if a direction $h$ has $rh>0$ everywhere on $M$, [compactness](../../../../../../compact-space.md) gives a positive lower bound on this product. On a sufficiently small neighborhood of $M$, $r$ and $h$ therefore have matching signs with $|h|$ bounded away from zero and $|r|$ bounded away from zero. On its compact complement, $|r|\le E-\delta$ for some $\delta>0$. Choose $\varepsilon>0$ so small that $\varepsilon\|h\|_\infty<\delta$ and that subtracting $\varepsilon h$ does not cross zero on that neighborhood. Then $\|r-\varepsilon h\|_\infty<E$, so $p$ is not a [best uniform approximation](../../../../../../best-uniform-approximation.md). This proves both directions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
