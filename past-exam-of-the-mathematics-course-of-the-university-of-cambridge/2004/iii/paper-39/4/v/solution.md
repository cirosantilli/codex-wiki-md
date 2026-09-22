<h1 id="4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $A=R_{11}+2R_{12}+R_{22}$. Among the ten complete trios, six have two heterozygous parents: three have child $11$, two have child $12$ and one has child $22$. Their [conditional likelihood](../../../../../../conditional-likelihood.md) contribution is

$$
\left(\frac{R_{11}}A\right)^3\left(\frac{2R_{12}}A\right)^2\frac{R_{22}}A=\frac{4R_{11}^3R_{12}^2R_{22}}{A^6}.
$$

Two more trios have a heterozygous parent and a $22$ parent, with child $12$ in each; they contribute $[R_{12}/(R_{12}+R_{22})]^2$. The remaining two parent pairs can produce only child $12$, so their conditional probabilities are one. Multiplying gives

$$
\boxed{L_{\rm exact}=\frac{4R_{11}^3R_{12}^4R_{22}}{(R_{11}+2R_{12}+R_{22})^6(R_{12}+R_{22})^2}.}
$$

The factor $4$ does not depend on the [genotype relative risks](../../../../../../genotype-relative-risk.md), so the conventional proportional [likelihood function](../../../../../../likelihood-function.md) is

$$
L\propto\frac{R_{11}^3R_{12}^4R_{22}}{(R_{11}+2R_{12}+R_{22})^6(R_{12}+R_{22})^2}.
$$

This is the expression in the original PDF, up to the parameter-independent constant. Its last denominator is $R_{12}+R_{22}$; the converted TeX's $R_{11}+R_{22}$ is a transcription error. The factor $4$ in the exact probability comes from the two heterozygous children of two heterozygous parents, each of which has two labelled transmission routes.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
