<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

There is a normalization error in the PDF. With the printed unnormalized integral, testing a constant function equal to one would give a left side $|U|(1-|U|)^2$ and a right side zero. Thus that formulation fails whenever $|U|\ne1$.

Use instead the average $v_U=|U|^{-1}\int_Uv$. The [Poincare-Wirtinger inequality](../../../../../../../poincare-wirtinger-inequality.md), also called the [Neumann-Poincare inequality](../../../../../../../poincare-wirtinger-inequality.md), is

$$
\boxed{\|v-v_U\|_{L^2(U)}^2\leq C_P\|\nabla v\|_{L^2(U)}^2.}
$$

If no $C_P$ exists, subtract the average and normalize a violating sequence to obtain $w_j\in H^1(U)$ with $\int_Uw_j=0$, $\|w_j\|_2=1$, and $\|\nabla w_j\|_2\to0$. This sequence is bounded in the [Sobolev space](../../../../../../../sobolev-space-split.md) $H^1(U)$. The [Rellich-Kondrachov compactness theorem](../../../../../../../rellich-kondrachov-theorem.md) supplies a subsequence converging strongly in $L^2(U)$ to $w$.

For every compactly supported [test function](../../../../../../../test-function.md) $\varphi$, [integration by parts](../../../../../../../integration-by-parts.md) and these convergences give $\int w\partial_i\varphi=0$. Thus $w$ has zero [weak gradient](../../../../../../../weak-gradient.md). The [Sobolev function with zero weak gradient](../../../../../../../sobolev-function-with-zero-weak-gradient.md) result and connectedness make $w$ constant. Strong $L^2$ convergence preserves its zero integral, so $w=0$. It also preserves its [norm](../../../../../../../norm.md) one, a contradiction. This proves the correctly normalized [Neumann-Poincare inequality](../../../../../../../poincare-wirtinger-inequality.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
