<h1 id="b/4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Expand both generating functions and use [orthogonality](../../../../../orthogonal-vectors.md) of the [Legendre polynomials](../../../../../legendre-polynomial.md), with $\int_{-1}^1P_nP_m=2\delta_{nm}/(2n+1)$. The allowed exchanges give

$$
\int_{-1}^1\frac{dt}{\sqrt{1-2wt+w^2}\sqrt{1-2zt+z^2}}=2\sum_{n\geq0}\frac{(wz)^n}{2n+1}.
$$

Hence it depends only on $r=wz$. Explicitly,

$$
\boxed{F(r)=2\int_0^1\frac{ds}{1-rs^2}=\begin{cases}2\operatorname{artanh}(\sqrt r)/\sqrt r,&r>0,\\2,&r=0,\\2\arctan(\sqrt{-r})/\sqrt{-r},&r<0.\end{cases}}
$$

The [series](../../../../../series-mathematics.md) form alone already proves the required dependence.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
