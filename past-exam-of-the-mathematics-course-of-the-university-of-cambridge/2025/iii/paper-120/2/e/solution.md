<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take

$$
\delta=\lambda x.\lambda f.f(xf).
$$

If $L$ is a [fixed-point combinator](../../../../../../fixed-point-combinator.md), then $Lf\equiv_\beta f(Lf)$, so eta-conversion gives

$$
L\equiv_\eta\lambda f.Lf\equiv_\beta\lambda f.f(Lf)=\delta L.
$$

Conversely, if $L\equiv_{\beta\eta}\delta L$, application to an arbitrary $f$ gives $Lf\equiv_{\beta\eta}f(Lf)$, which is precisely the fixed-point-combinator property.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
