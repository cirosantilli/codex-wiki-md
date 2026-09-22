<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

The [chain rule](../../../../../chain-rule.md) along the specified straight line gives

$$
F'(0)=\alpha f_1(a,b)+\beta f_2(a,b),\qquad
F''(0)=\alpha^2f_{11}(a,b)+2\alpha\beta f_{12}(a,b)+\beta^2f_{22}(a,b).
$$

Here equality of mixed [partial derivatives](../../../../../partial-derivative.md) follows from smoothness. Apply [Taylor theorem](../../../../../taylor-theorem.md) in the single variable $t$:

$$
F(t)=F(0)+tF'(0)+\tfrac12t^2F''(0)+o(t^2).
$$

Writing $h_1=x_1-a=\alpha t$ and $h_2=x_2-b=\beta t$ produces the linear and quadratic terms

$$
f(a+h_1,b+h_2)=f(a,b)+h_1f_1+h_2f_2
+\tfrac12(h_1^2f_{11}+2h_1h_2f_{12}+h_2^2f_{22})+o(|h|^2),
$$

with all displayed [partial derivatives](../../../../../partial-derivative.md) evaluated at $(a,b)$. For a remainder valid uniformly over directions, apply the [Taylor formula with integral remainder](../../../../../taylor-formula-with-integral-remainder.md) to $s\mapsto f((a,b)+sh)$:

$$
f((a,b)+h)=f(a,b)+\nabla f(a,b)\cdot h
+\int_0^1(1-s)h^TH((a,b)+sh)h\,ds.
$$

Continuity of the [Hessian matrix](../../../../../hessian-matrix.md) makes the difference between the integral and $\tfrac12h^TH(a,b)h$ be $o(|h|^2)$. The printed ellipsis is therefore justified as a finite [Taylor expansion](../../../../../taylor-expansion.md) with a remainder. Smoothness alone does not assert convergence of an infinite [Taylor series](../../../../../taylor-series.md).

At a [stationary point](../../../../../stationary-point.md), the linear term vanishes. The symmetric [Hessian matrix](../../../../../hessian-matrix.md) satisfies

$$
h^THh
=H_{11}\left(h_1+\frac{H_{12}}{H_{11}}h_2\right)^2
+\frac{\det H}{H_{11}}h_2^2.
$$

If $H_{11}>0$ and $\det H>0$, this is a [positive-definite quadratic form](../../../../../positive-definite-quadratic-form.md). Its minimum over the [unit circle](../../../../../complex-unit-circle.md) is a positive number $c$, so $h^THh\geq c|h|^2$. The [Taylor remainder](../../../../../taylor-remainder.md) is smaller than $c|h|^2/4$ for sufficiently small $h$, proving $f((a,b)+h)>f(a,b)$ for nonzero nearby $h$. Thus **the stationary point is a strict local minimum**.

For the given polynomial, the [gradient](../../../../../gradient.md) equations reduce to

$$
x_2=-x_1,\qquad 4x_1(x_1^2-1)=0.
$$

The [stationary points](../../../../../stationary-point.md) are $(0,0),(1,-1),(-1,1)$, and

$$
H=\begin{pmatrix}12x_1^2-2&2\\2&2\end{pmatrix}.
$$

At both points with $x_1=\pm1$, we have $H_{11}=10>0$ and $\det H=16>0$. Consequently

$$
\boxed{(1,-1)\text{ and }(-1,1)\text{ are local minima, with }f=-1.}
$$

At the origin the [determinant](../../../../../determinant.md) of the [Hessian matrix](../../../../../hessian-matrix.md) is $-8$, giving a [saddle point](../../../../../saddle-point.md). An independent check is the identity $f=(x_1^2-1)^2+(x_1+x_2)^2-1$, which proves that the two displayed [local minima](../../../../../local-minimum.md) are also the only global minima.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
