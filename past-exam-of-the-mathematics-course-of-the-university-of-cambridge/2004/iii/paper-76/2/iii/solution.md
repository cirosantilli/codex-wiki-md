<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

By [Stirling's approximation](../../../../../../stirling-formula.md), for fixed $a$,

$$
\frac{\Gamma(r+a)}{\Gamma(r)}=r^a[1+O(r^{-1})].
$$

Apply this with $a=1/6,5/6$ and use $\Gamma(r+1)=r\Gamma(r)$. Their exponents add to one, and hence

$$
\boxed{Y_r=\frac{\Gamma(r)}{2\pi\sigma^r}[1+O(r^{-1})]}.
$$

More explicitly, the ratio is $1-5/(36r)+O(r^{-2})$. The exact ratio of neighboring terms is

$$
\frac{Y_{r+1}}{Y_r}=\frac{(r+1/6)(r+5/6)}{\sigma(r+1)}\sim\frac r\sigma.
$$

Thus the [Airy function](../../../../../../airy-function.md) expansion is factorially divergent, and [optimal truncation](../../../../../../optimal-truncation.md) retains about $|\sigma|$ terms.

**The printed summation starts at $r=1$, but its leading $r=0$ term is missing.** The [Gamma reflection formula](../../../../../../gamma-reflection-formula.md) gives $\Gamma(1/6)\Gamma(5/6)=2\pi$, so $Y_0=1$. The correctly normalized dominant [Airy function](../../../../../../airy-function.md) expansion starts at zero. This correction is essential for the exponentially small remainder in the next part; if the printed series is used literally, its remainder also contains the entire missing leading term.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
