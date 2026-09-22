<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the principal [branch of the complex logarithm](../../../../../branch-of-the-complex-logarithm.md) for $\operatorname{Log}(z+i)$. Its [branch cut](../../../../../branch-cut.md) is the ray $z=-i-s$, $s\geq0$, lying below the real axis. Thus it is analytic in the upper half-plane, where the only [pole](../../../../../pole.md) of the integrand is $z=i$.

Close the real interval by a large upper semicircle. The [estimation lemma](../../../../../estimation-lemma.md) bounds the arc integral by $O(\ln R/R)$, so it vanishes. The simple-pole [residue](../../../../../residue.md) is

$$
\operatorname{Res}_{z=i}\frac{\operatorname{Log}(z+i)}{z^2+1}=\frac{\operatorname{Log}(2i)}{2i}=\frac{\ln2+i\pi/2}{2i}.
$$

The [residue theorem](../../../../../residue-theorem.md) then gives

$$
\int_{-\infty}^{\infty}\frac{\operatorname{Log}(x+i)}{x^2+1}dx=\pi\ln2+\frac{i\pi^2}{2}.
$$

For real $x$, $\operatorname{Re}\operatorname{Log}(x+i)=\tfrac12\ln(x^2+1)$. Taking real parts and then using evenness of the real integrand yields

$$
\boxed{\int_0^\infty\frac{\ln(x^2+1)}{x^2+1}dx=\pi\ln2.}
$$

Both endpoints converge: the integrand is $O(x^2)$ near zero and $O(\ln x/x^2)$ at infinity. This also agrees with the [logarithmic parameter integral with Cauchy weight](../../../../../logarithmic-parameter-integral-with-cauchy-weight.md) at parameter one.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
