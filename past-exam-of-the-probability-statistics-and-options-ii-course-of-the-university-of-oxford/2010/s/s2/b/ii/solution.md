<h1 id="s/s2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $x\ne0$, the envelope ratio is

$$
\frac{p(x)}{q(x)}=\frac32(1+x^2)\left(\frac{\sin x}x\right)^4.
$$

If $|x|\le1$, use $|\sin x|\le|x|$ to bound this by $\tfrac32(1+x^2)\le3$. If $|x|\ge1$, use $|\sin x|\le1$ to bound it by $\tfrac32(x^{-4}+x^{-2})\le3$. The boundary equalities in these bounds cannot both occur in the sine estimate, so $M=3$ is a valid envelope. At zero the [continuous](../../../../../../continuous-function.md) ratio is $3/2$.

Generate [independent](../../../../../../independent-random-variables.md) [Cauchy](../../../../../../cauchy-sequence.md) proposals as in (i), together with [independent](../../../../../../independent-random-variables.md) uniform $U$. Accept a proposal $Y$ when

$$
\boxed{U\le\tfrac12(1+Y^2)\left(\frac{\sin Y}{Y}\right)^4,}
$$

using the limiting value $1/2$ at $Y=0$. Repeat until acceptance. Part (a) proves exactness; the overall acceptance rate is $1/3$ and the mean number of proposals is three. No numerical maximization of the ratio is needed for correctness.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [S2](../../../s2.md)
4. [S](../../../../s.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
