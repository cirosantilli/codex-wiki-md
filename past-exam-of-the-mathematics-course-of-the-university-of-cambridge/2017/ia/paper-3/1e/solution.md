<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

Use the [Riemann sphere](../../../../../riemann-sphere.md) convention for evaluating a [Möbius transformation](../../../../../mobius-transformation.md) at a pole and at infinity. When the three prescribed points are finite, take

$$
f(z)=\frac{(w_3-w_1)(z-w_2)}{(w_3-w_2)(z-w_1)}.
$$

Its zero is $w_2$, its pole is $w_1$, and substitution at $w_3$ gives one. The remaining three cases are

$$
\boxed{
\begin{array}{c|c}
\text{point at infinity}&f(z)\\ \hline
w_1=\infty&(z-w_2)/(w_3-w_2)\\
w_2=\infty&(w_3-w_1)/(z-w_1)\\
w_3=\infty&(z-w_2)/(z-w_1).
\end{array}}
$$

All coefficient [determinants](../../../../../determinant.md) are nonzero because the points are distinct. There is only one such [Möbius transformation](../../../../../mobius-transformation.md): the composite of any two candidate maps, one inverted, fixes $\infty,0,1$; fixing infinity makes it affine, and fixing zero and one makes it the identity.

For this question use the [cross-ratio](../../../../../cross-ratio.md) normalization

$$
\boxed{[w_1,w_2,w_3,w_4]=f(w_4).}
$$

In the finite case this is $(w_3-w_1)(w_4-w_2)/[(w_3-w_2)(w_4-w_1)]$, with the corresponding limits if a point is infinite. It is finite and distinct from zero and one, since $w_4$ is distinct from the other three points and $f$ is a [bijection](../../../../../bijection.md). Ordering conventions for the [cross-ratio](../../../../../cross-ratio.md) differ; the definition here is fixed by the specified images, rather than by importing another ordering formula.

A [generalized circle](../../../../../generalized-circle-under-a-mobius-transformation.md) means either a [circle](../../../../../circle.md) or a [straight line](../../../../../straight-line.md) completed by infinity. Let $K$ be the unique [generalized circle](../../../../../generalized-circle-under-a-mobius-transformation.md) through the first three points. Its image under $f$ is the unique [generalized circle](../../../../../generalized-circle-under-a-mobius-transformation.md) through $\infty,0,1$, namely $\mathbb R\cup\{\infty\}$. Therefore $w_4\in K$ exactly when $f(w_4)$ is real. Conversely a real $f(w_4)$ lies on that extended real line, whose inverse image is $K$. This proves the [real cross-ratio criterion for a generalized circle](../../../../../real-cross-ratio-criterion-for-a-generalized-circle.md) in both directions.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
