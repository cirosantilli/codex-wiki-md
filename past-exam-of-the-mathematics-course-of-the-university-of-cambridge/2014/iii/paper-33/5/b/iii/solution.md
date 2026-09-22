<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The trace of the smoother's influence matrix is its total [effective degrees of freedom](../../../../../../../effective-degrees-of-freedom.md). Include the unpenalized intercept as well as both centered smooth terms:

$$
\boxed{\operatorname{tr}(A)=1+1.257+1.895\approx4.152.}
$$

The `Ref.df` entries are for approximate significance calibration and must not be summed to obtain this trace. A consistency check using the [generalized cross-validation](../../../../../../../generalized-cross-validation.md) form $nD/(n-\operatorname{tr}A)^2$ and scale estimate $D/(n-\operatorname{tr}A)$ gives $\operatorname{tr}A\approx200(1-3.3506/3.4217)\approx4.16$; the small difference is explained by rounding in the displayed quantities. **The required trace is about $4.15$.**

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
