<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**About five steps are certified by the uniform worst-case estimate; the actual iteration reaches double-precision accuracy in about four.** Put $K=15/14$. The initial enclosure gives $e_0=|x_0-r|<1/5$, and repeated squaring yields

$$
e_k\le\frac1K(Ke_0)^{2^k}
<\frac{14}{15}\left(\frac3{14}\right)^{2^k}.
$$

For $k=4$ this is about $1.84\times10^{-11}$, while for $k=5$ it is below $4\times10^{-22}$. Thus five ideal-arithmetic steps push this bound well below the approximately $10^{-16}$ relative resolution of [double-precision floating-point format](../../../../../../double-precision-floating-point-format.md).

The bound is conservative. Factoring $f(x)=(x^2+1)(x^4-6x^2+6)$ identifies

$$
r=\sqrt{3-\sqrt3}\approx1.126032500610494238.
$$

High-precision evaluation of the actual successive errors gives approximately $7.40\times10^{-2}$, $3.56\times10^{-3}$, $9.91\times10^{-6}$, $7.73\times10^{-11}$ and $4.70\times10^{-21}$. Thus the fourth step would already exceed double-precision accuracy in exact arithmetic. In floating-point evaluation, cancellation in the residual and other [roundoff errors](../../../../../../round-off-error.md) prevent the subsequent theoretical digits from being realized.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
