<h1 id="32e/solution">Solution</h1>

↑ **Parent:** [32E](../32e.md)

A [Poisson structure](../../../../../poisson-structure.md) is a smooth antisymmetric [matrix](../../../../../matrix.md) field $\omega^{ab}$ defining a bracket

$$
\{f,g\}=\sum_{a,b}\omega^{ab}\partial_af\,\partial_bg
$$

that obeys the [Jacobi identity](../../../../../jacobi-identity.md). Bilinearity, antisymmetry and the product rule follow from this formula; Jacobi is the remaining condition. Applying Jacobi to the coordinate functions gives

$$
\boxed{\sum_d\left(\omega^{dc}\partial_d\omega^{ab}
+\omega^{db}\partial_d\omega^{ca}
+\omega^{da}\partial_d\omega^{bc}\right)=0.}
$$

These are also sufficient: expanding Jacobi for arbitrary functions cancels all second-derivative terms by antisymmetry, leaving these coefficients multiplying their first derivatives.

For $\omega^{ab}=\epsilon^{abc}x^c$, the nonconstant function $f=\sum_a(x^a)^2$ is a [Casimir function of a Poisson manifold](../../../../../casimir-function-of-a-poisson-manifold.md), because

$$
\{f,x^a\}=2\sum_{b,c}x^b\epsilon^{bac}x^c=0
$$

by symmetry of $x^bx^c$. This is the usual three-dimensional [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md).

Since the [matrix](../../../../../matrix.md) $M$ is symmetric, $\partial_dH=\sum_bM^{db}x^b$. The [Hamilton equations](../../../../../hamilton-s-equations.md) are $\dot x^a=\{x^a,H\}$, and hence

$$
\dot x^a=\sum_{b,c,d}\epsilon^{adc}M^{db}x^bx^c.
$$

One valid choice of coefficients is $Q^{abc}=\sum_d\epsilon^{adc}M^{db}$. If symmetric coefficients in $b,c$ are preferred, the same equations use

$$
\boxed{Q^{abc}=\frac12\sum_d
\left(\epsilon^{adc}M^{db}+\epsilon^{adb}M^{dc}\right).}
$$

In vector notation the evolution is $(Mx)\times x$, consistent with the bracket convention and with preservation of $|x|^2$.

## ↑ Ancestors (10)

1. [32E](../32e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
