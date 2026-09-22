<h1 id="2/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\omega=\theta^{-1}(\alpha)$. The preceding invariant formula for the [exterior derivative](../../../../../../exterior-derivative.md) identifies the expression in the question with

$$
X(\alpha(Y))-Y(\alpha(X))-\alpha([X,Y])=d\omega(X,Y).
$$

Its vanishing for every pair of global [vector fields](../../../../../../vector-field.md) is equivalent to $d\omega=0$: global fields with arbitrary prescribed tangent values are available by bump-function extension. Thus it is exactly the condition that $\omega$ be a [closed differential one-form](../../../../../../closed-differential-one-form.md).

By definition, the first [de Rham cohomology](../../../../../../de-rham-cohomology.md) is closed one-forms modulo [exact differential forms](../../../../../../exact-differential-form.md). The hypothesis $H^1_{\mathrm{dR}}(M)=0$ makes every closed one-form exact. Hence $d\omega=0$ gives a globally smooth function $g$ with $\omega=dg$, and

$$
\boxed{\alpha(X)=dg(X)=X(g)\quad\text{for every }X.}
$$

Conversely, if $\alpha(X)=X(g)$, then

$$
X(\alpha(Y))-Y(\alpha(X))-\alpha([X,Y])
=X(Yg)-Y(Xg)-[X,Y]g=0
$$

by the definition of the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md). Equivalently, $d(dg)=0$. **The bracket compatibility condition is necessary and, when $H^1_{\mathrm{dR}}(M)=0$, sufficient for a global potential.** The potential is unique up to a constant on each connected component, since the difference of two potentials has zero differential.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
