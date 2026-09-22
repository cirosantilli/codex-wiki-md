<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Model m1 is [ridge regression](../../../../../../ridge-regression.md), while m2 is the [Lasso](../../../../../../lasso.md). Ridge shrinks but normally retains every coefficient; the Lasso's $\ell^1$ penalty sets many coefficients exactly to zero. Model m3 combines sparsity with the [grouping effect of the elastic net](../../../../../../grouping-effect-of-the-elastic-net.md): correlated predictors tend to enter together and receive more similar coefficients.

Accordingly, m3 keeps the weak variables age, lcp, and gleason at zero as m2 does, but retains lweight, lbph, svi, and pgg45 as the ridge fit does. The correlation $0.54$ between svi and lcavol explains why m3 keeps both with substantial coefficients, whereas m2 selects lcavol and discards svi. This lies between the dense ridge behavior and the more aggressively sparse Lasso behavior.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
