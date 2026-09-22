<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [digital call option](../../../../../../digital-call-option.md) and [digital put option](../../../../../../digital-put-option.md) indicators partition the possible terminal stock prices:

$$
\mathbf1_{\{S_T\geq K\}}
+\mathbf1_{\{S_T<K\}}=1.
$$

Thus the [digital put-call parity](../../../../../../digital-put-call-parity.md) is

$$
\boxed{
D_{\rm call}(t,S_t)+D_{\rm put}(t,S_t)
=e^{-r(T-t)}.}
$$

At time zero, part b gives $D_{\rm call}(0,S_0)=e^{-rT}\Phi(d_-)$, so

$$
\boxed{
D_{\rm put}(0,S_0)
=e^{-rT}\bigl(1-\Phi(d_-)\bigr)
=e^{-rT}\Phi(-d_-).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
