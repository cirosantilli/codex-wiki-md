<h1 id="6e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a stable one-species [linear noise approximation](../../../../../../linear-noise-approximation.md), the [normalized stationary fluctuation-dissipation relation for a reaction network](../../../../../../normalized-stationary-fluctuation-dissipation-relation-for-a-reaction-network.md) becomes

$$
\boxed{\eta=\frac{\operatorname{Var}x}{m^2}
=\frac{\langle r\rangle}{Hm}.}
$$

To see the factors explicitly, the linearized restoring rate is $a=H/\tau=4\beta m$, while the chemical noise intensity is the rate-weighted squared step size

$$
B=\lambda\cdot1^2+\beta m^2\cdot(-2)^2=3\lambda.
$$

Stationarity of the [variance](../../../../../../variance-split.md) gives $2a\operatorname{Var}x=B$. Using $\lambda=2\beta m^2$ therefore yields

$$
\operatorname{Var}x=\frac{3m}{4},\qquad
\boxed{\eta=\frac3{4m}=\frac3{4\langle x\rangle}.}
$$

This is the stationary fluctuation result within the stated negligible-fluctuation/linear-noise approximation, not an exact identity for the boundary-corrected discrete chemistry.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6E](../../6e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
