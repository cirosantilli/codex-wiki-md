<h1 id="22f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $f=\mathbf1_{[0,1]}$. Its [Fourier transform](../../../../../../fourier-transform.md) is

$$
\widehat f(\xi)=e^{-\pi i\xi}\frac{\sin(\pi\xi)}{\pi\xi},
$$

with value one at zero. It is bounded near zero and is $O(|\xi|^{-1})$ at infinity, so $(1+\xi^2)^s|\widehat f|^2=O(|\xi|^{2s-2})$ is integrable for $s<1/2$. Therefore

$$
\boxed{\mathbf1_{[0,1]}\in H^s(\mathbb R)\quad(0<s<1/2).}
$$

If a [continuous function](../../../../../../continuous-function.md) agreed with this indicator [almost everywhere](../../../../../../almost-everywhere.md), [continuity](../../../../../../continuous-function.md) would force it to equal zero on $(-\infty,0)$ and one on $(0,1)$: any violation has a nonempty open neighbourhood of [positive measure](../../../../../../positive-measure.md). The one-sided limits at zero would then differ, a contradiction. Hence no continuous representative exists.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [22F](../../22f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
