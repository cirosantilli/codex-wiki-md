<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For smooth $u$, the fundamental theorem along the segment in direction $e_k$ gives, for either sign of $h$,

$$
\Delta_k^h u(x)=\int_0^1D_k u(x+the_k)\,dt.
$$

The entire segment lies in $\Omega$ under the distance hypothesis. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) on $[0,1]$, followed by integration and translation, yields

$$
\int_{\Omega'}|\Delta_k^h u|^2\leq\int_0^1\int_{\Omega'}|D_k u(x+the_k)|^2\,dx\,dt
\leq\int_\Omega|D_k u|^2\leq\int_\Omega|Du|^2.
$$

For general $u\in W^{1,2}(\Omega)$, extend $u$ and its weak [gradient](../../../../../../gradient.md) separately by zero as $L^2$ functions on $\mathbb R^n$, and mollify $u$ with radius $\varepsilon$. At points farther than $\varepsilon$ from the boundary the mollified [gradient](../../../../../../gradient.md) equals the [convolution](../../../../../../convolution.md) of the zero-extended [gradient](../../../../../../gradient.md), because the [convolution](../../../../../../convolution.md) kernel is supported wholly inside $\Omega$. Choose $\varepsilon<\operatorname{dist}(\Omega',\partial\Omega)-|h|$. All the segments then lie in this region, and the preceding calculation, followed by the $L^2$ contraction bound for [convolution](../../../../../../convolution.md), gives the same right side $\|D_k u\|_{L^2(\Omega)}$. The [mollifications](../../../../../../mollification.md) converge locally in $L^2$, as do their fixed-$h$ translated differences, so passage to the limit preserves the estimate. Hence

$$
\boxed{\Delta_k^h u\in L^2(\Omega'),\qquad\|\Delta_k^h u\|_{L^2(\Omega')}\leq\|Du\|_{L^2(\Omega)}.}
$$

The argument proves the sharper estimate with $D_k u$ on the right. It is the basic Sobolev [difference quotient](../../../../../../difference-quotient.md) bound.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
