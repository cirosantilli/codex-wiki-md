# Logarithmic beta integral from a sector contour

↑ **Parent:** [Residue theorem](residue-theorem.md)

For real $\beta>1$, choose a [branch of the complex logarithm](branch-of-the-complex-logarithm.md) whose argument interval contains $[0,2\pi/\beta]$ strictly, and integrate $\operatorname{Log}z/(1+z^\beta)$ over an annular sector of angle $\alpha=2\pi/\beta$. The one enclosed [simple pole](simple-pole.md) is $e^{i\pi/\beta}$, with [residue](residue.md) $-i\pi e^{i\pi/\beta}/\beta^2$. The circular arcs tend to zero, with bounds $O(\epsilon|\log\epsilon|)$ and $O(R^{1-\beta}\log R)$.

Writing $I$ for the title integral and $J=\int_0^\infty(1+x^\beta)^{-1}dx$, the two radial segments and the [residue theorem](residue-theorem.md) give

$$
(1-e^{i\alpha})I-i\alpha e^{i\alpha}J=\frac{2\pi^2}{\beta^2}e^{i\pi/\beta}.
$$

Divide by $e^{i\pi/\beta}$ and equate real and imaginary parts. This gives $J=\pi/[\beta\sin(\pi/\beta)]$ and the title formula. When $1<\beta<2$, the sector extends below the negative real axis; the [principal complex logarithm](principal-complex-logarithm.md) therefore cannot be used throughout that sector. A cut along a ray just below the positive axis avoids this issue for every $\beta>1$.

## ↑ Ancestors (5)

1. [Residue theorem](residue-theorem.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/4/solution.md)
