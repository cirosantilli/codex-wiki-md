<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The derivative of the backward [characteristic flow map](../../../../../../characteristic-flow-map.md) is

$$
 DS_{0,t}=\begin{pmatrix}\cosh t&-\sinh t\\-\sinh t&\cosh t\end{pmatrix},
 \qquad \boxed{\det DS_{0,t}=\cosh^2t-\sinh^2t=1.}
$$

Thus the [change of variables formula](../../../../../../change-of-variables-formula.md) preserves phase-space [Lebesgue measure](../../../../../../lebesgue-measure.md). With zero source, $f_t=f_0\circ S_{0,t}$, so for every finite $p>0$,

$$
 \int_{\mathbb R^2}|f_t(x,v)|^p\,dx\,dv
 =\int_{\mathbb R^2}|f_0(x_0,v_0)|^p\,dx_0\,dv_0.
$$

Taking the $p$th root proves **$\|f_t\|_p=\|f_0\|_p$**. For $0<p<1$ this is a [quasi-norm](../../../../../../quasi-norm.md), and the argument still works because it uses only a change of variables, not the [triangle inequality](../../../../../../triangle-inequality.md). The identity also holds in the extended sense when an [integral](../../../../../../integral.md) is infinite. Since the flow is bijective and measure-preserving, it additionally preserves the [essential supremum](../../../../../../essential-supremum.md), so the same conclusion holds for $p=\infty$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
