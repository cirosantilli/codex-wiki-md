<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Independently generate $U$ uniform on $(0,1)$ and $V$ uniform on $(b_1,b_2)$, using the bounds above. Accept the proposal if

$$
U^2\leq\exp\left(-\frac{|V/U-1|}{2}\right);
$$

otherwise generate a fresh pair. On acceptance return $X=V/U$. The bounding rectangle contains the entire ratio region: $U\leq\sqrt{h(X)}\leq a$, and $V=XU$ lies between the extrema of $x\sqrt{h(x)}$. Conditioning a uniform rectangle point on acceptance makes it uniform on $C_h$, so the preceding [marginal distribution](../../../../../../../marginal-distribution.md) calculation proves that the returned value has the desired [Laplace distribution](../../../../../../../laplace-distribution.md).

For this target $H=4$, so the region has area two. The [rejection sampling](../../../../../../../rejection-sampling.md) acceptance [probability](../../../../../../../probability.md) is

$$
\boxed{\frac{2}{4(e^{-3/4}+e^{-5/4})}=\frac{1}{2(e^{-3/4}+e^{-5/4})}.}
$$

Endpoints have zero [probability](../../../../../../../probability.md) and can be excluded to avoid divisions by zero in implementation.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
