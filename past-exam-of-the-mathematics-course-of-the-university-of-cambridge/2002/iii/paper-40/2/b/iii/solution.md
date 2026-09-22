<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $x\geq k$, the proposal CDF is $G(x)=1-k/x$. Therefore [inverse transform sampling](../../../../../../../inverse-transform-sampling.md) with $V\sim U(0,1)$ gives

$$
X=G^{-1}(V)=\frac{k}{1-V}.
$$

Equivalently, put $U=1-V$, which is also uniform, and use **$X=k/U$**. This equivalent parametrization matches the uniforms used in the final [estimator](../../../../../../../estimator.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
