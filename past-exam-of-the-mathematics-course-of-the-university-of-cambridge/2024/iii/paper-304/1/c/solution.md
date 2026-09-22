<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Inside the [generating functional](../../../../../../generating-functional.md), multiplication by a field can be replaced by a [functional derivative](../../../../../../functional-derivative.md) of the source factor:

$$
\phi(x)e^{i\int J\phi}=\frac1i\frac{\delta}{\delta J(x)}e^{i\int J\phi}
=-i\frac{\delta}{\delta J(x)}e^{i\int J\phi}.
$$

Expanding the interaction exponential, making this replacement in every term, and resumming gives

$$
\boxed{
Z_n[J]=\exp\!\left[-ig\frac{(-i)^n}{n!}
\int d^dx\,\frac{\delta^n}{\delta J(x)^n}\right]Z_0[J]}.
$$

This formal identity assumes a common regulator, a source-independent normalization, and permission to interchange the [path integral](../../../../../../path-integral.md), power series, and functional derivatives. A normalized functional with $Z_n[0]=1$ requires division by the same expression evaluated at $J=0$, which removes connected [Vacuum Feynman diagrams](../../../../../../vacuum-feynman-diagram.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
