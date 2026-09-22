<h1 id="13c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a [variation](../../../../../../variation.md) $y+\varepsilon\eta$, where the [differentiable function](../../../../../../differentiable-function.md) $\eta$ obeys

$$
\eta(a)=\eta(b)=\eta'(a)=\eta'(b)=0
$$

because both $y$ and its first [derivative](../../../../../../derivative.md) have fixed endpoint values. The [first variation](../../../../../../first-variation.md) of the [functional](../../../../../../functional.md) is

$$
\delta L
=\int_a^b
\left(F_y\eta+F_{y'}\eta'+F_{y''}\eta''\right)\,dx.
$$

Applying [integration by parts](../../../../../../integration-by-parts.md) once to the second term and twice to the third gives

$$
\begin{aligned}
\delta L
={}&\int_a^b
\left[
F_y-\frac d{dx}F_{y'}
+\frac{d^2}{dx^2}F_{y''}
\right]\eta\,dx\\
&+\left[
F_{y'}\eta+F_{y''}\eta'
-\frac d{dx}(F_{y''})\eta
\right]_a^b.
\end{aligned}
$$

The endpoint conditions on $\eta$ and $\eta'$ make every boundary term zero. Since the remaining [integral](../../../../../../integral.md) vanishes for every admissible variation, the [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) yields the [higher-order Euler-Lagrange equation](../../../../../../higher-order-euler-lagrange-equation.md)

$$
\boxed{
F_y-\frac d{dx}F_{y'}
+\frac{d^2}{dx^2}F_{y''}=0
}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13C](../../13c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
