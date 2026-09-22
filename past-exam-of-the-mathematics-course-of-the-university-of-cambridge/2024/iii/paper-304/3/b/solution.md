<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The disjoint Fourier supports make the quadratic cross term $\int\partial\phi\cdot\partial\chi$ vanish. Therefore

$$
S[\phi+\chi]=S[\phi]+S_{0,\chi}[\chi]+S_{\rm int}[\phi,\chi],
$$

where

$$
\boxed{S_{\rm int}[\phi,\chi]=\frac g{3!}\int d^dx
\left(3\phi^2\chi+3\phi\chi^2+\chi^3\right)}.
$$

Define the high-mode free [generating functional](../../../../../../generating-functional.md) with source convention

$$
Z_\chi[J]=\int\mathcal D\chi\,
e^{-S_{0,\chi}[\chi]-\int J\chi}.
$$

Then inserting $\chi=-\delta/\delta J$ reproduces every high-field factor, and

$$
\boxed{e^{-W[\phi]}=e^{-S[\phi]}
\left.e^{-S_{\rm int}[\phi,-\delta/\delta J]}Z_\chi[J]\right|_{J=0}}.
$$

Expanding the interaction exponential and applying [Wick theorem](../../../../../../wick-s-theorem.md) evaluates the [Wilsonian effective action](../../../../../../wilsonian-effective-action.md) as a sum of connected diagrams whose internal lines are restricted to the high-momentum shell.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
