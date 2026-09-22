<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A stable multiplicative sensitivity factor $s_i$ at [detector pixel](../../../../../../../optical-detector-pixel.md) $i$ changes both means to $N_i=s_iN_0$. The noise-free ratio is still one, so [flat-field correction](../../../../../../../flat-field-correction.md) is not required merely to remove that fixed pattern from the mean ratio. This is the principal advantage of using two matched flats rather than the [variance](../../../../../../../variance-split.md) of a single image.

However, the [photon shot noise](../../../../../../../photon-shot-noise.md) is not cancelled. At high counts the conditional ratio [variance](../../../../../../../variance-split.md) is $2/(gN_i)$. Pooling [detector pixels](../../../../../../../optical-detector-pixel.md) gives $E^2\simeq(2/g)\langle1/N_i\rangle$, where brackets denote a spatial average. If the formula uses $\overline N=\langle N_i\rangle$, it returns

$$
\boxed{g_{\rm naive}\simeq\frac{g}{\langle N_i\rangle\langle1/N_i\rangle}\le g.}
$$

The inequality follows from the [Jensen inequality](../../../../../../../jensen-s-inequality.md) for $1/x$ on positive signals. For small fractional response variation, the relative bias is approximately minus its squared [coefficient of variation](../../../../../../../coefficient-of-variation.md). A locally nearly uniform region or a fit using [detector pixel](../../../../../../../optical-detector-pixel.md)-dependent [variances](../../../../../../../variance-split.md) avoids this bias from mixing the [harmonic mean](../../../../../../../harmonic-mean.md) with the [arithmetic mean](../../../../../../../arithmetic-mean.md). Stable response cancellation also presumes the conversion gain itself is uniform; gain variations, offset errors or changing sensitivity do not obey that simple cancellation. **The fixed response pattern cancels in the ratio mean; unequal shot-noise levels can still bias a globally pooled gain estimate.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
