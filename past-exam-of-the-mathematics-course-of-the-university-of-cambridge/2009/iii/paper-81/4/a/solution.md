<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With zero fluid [velocity](../../../../../../velocity.md) and all mean orientations vertical, the steady [cell conservation equation](../../../../../../cell-conservation-in-a-swimming-suspension.md) is

$$
\frac{d}{d\hat z}\left(V_s\hat n-D\frac{d\hat n}{d\hat z}\right)=0.
$$

The plates are impermeable to cells, so the constant vertical flux is zero. Hence $D\hat n_{\hat z}=V_s\hat n$, giving $\hat n=C\exp(V_s\hat z/D)$. Determine $C$ by the prescribed depth average:

$$
\frac1H\int_{-H}^0\hat n\,d\hat z=\hat n_0.
$$

With $z=\hat z/H$ and $h=V_sH/D$, the result is

$$
\boxed{\hat n=\hat n_0\bar n(z),\qquad\bar n(z)=\frac{he^{hz}}{1-e^{-h}}.}
$$

The same normalized profile describes cell number density or cell volume fraction, because cell volume is constant. Its weak-stratification expansion is

$$
\bar n=1+h\left(z+\frac12\right)+h^2\left(\frac{z^2}2+\frac z2+\frac1{12}\right)+O(h^3),
$$

which is depth-normalized at each displayed order and will be used in part (c). Upward swimming makes concentration larger near the upper plate, creating the density stratification responsible for [bioconvection](../../../../../../bioconvection.md) when cells are heavier than the fluid.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
