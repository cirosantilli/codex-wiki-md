<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose an [affine open subscheme](../../../../affine-open-subscheme.md) $V=\operatorname{Spec}A\subseteq Y$ containing $y$. Since $f$ is an [affine morphism](../../../../affine-morphism.md), $f^{-1}V=\operatorname{Spec}B$; by hypothesis $B$ is a [finitely generated module](../../../../finitely-generated-module.md) over $A$. If $\mathfrak m\subset A$ corresponds to the [closed point](../../../../closed-point.md) $y$, then $\kappa(y)=A/\mathfrak m$. The [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) is

$$
X_y=X\times_Y\operatorname{Spec}\kappa(y)
\cong\operatorname{Spec}\bigl(B\otimes_A\kappa(y)\bigr)
=\operatorname{Spec}(B/\mathfrak mB).
$$

If $b_1,\ldots,b_r$ generate the $A$-[module](../../../../module-mathematics.md) $B$, their images span the [algebra](../../../../algebra-split.md) $B/\mathfrak mB$ as a [vector space](../../../../vector-space-split.md) over $\kappa(y)$. It is therefore finite-dimensional. By the allowed fact about the [spectrum of a finite-dimensional commutative algebra](../../../../spectrum-of-a-finite-dimensional-commutative-algebra.md), it has only finitely many [prime ideals](../../../../prime-ideal.md). These are exactly the points of $X_y$, so

$$
\boxed{|f^{-1}(y)|=|\operatorname{Spec}(B/\mathfrak mB)|<\infty.}
$$

The points of the [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) correspond to the [prime ideals](../../../../prime-ideal.md) of $B$ contracting to $\mathfrak m$, which explains the equality with the underlying set-theoretic [fiber](../../../../fiber-of-a-function.md). An empty [fiber](../../../../fiber-of-a-function.md) is allowed. In fact, replacing $A/\mathfrak m$ by $\kappa(y)$ gives the same finite-dimensional argument for every point, without requiring it to be a [closed point](../../../../closed-point.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
