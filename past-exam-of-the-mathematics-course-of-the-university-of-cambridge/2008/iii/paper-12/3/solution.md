<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write the [rational function](../../../../../rational-function.md) $A$ in reduced form. We first exclude a finite pole in its dependent variable at a generic point $(a,b)$. If this pole has order $m\ge1$, the inverse equation

$$
\frac{dz}{dw}=\frac1{A(z,w)},\qquad z(b)=a,
$$

has a [holomorphic](../../../../../complex-differentiability-at-a-point.md) right-hand side near $(a,b)$, with a zero of order $m$ in $w-b$ at $z=a$. Choosing a generic point avoids collisions of pole branches and zeros of the reduced numerator. The unique inverse solution has

$$
z(w)-a=c(w-b)^{m+1}+O((w-b)^{m+2}),\qquad c\ne0.
$$

To justify the leading order, first note $z'(b)=0$; if the first nonzero term has order $\ell$, substitution in the inverse equation makes the right-hand side start at order $m$, since the change caused by $z-a$ has order at least $\ell$. Thus $\ell-1=m$. Inverting produces an [algebraic branch point](../../../../../algebraic-branch-point.md) of order $m+1$. Away from the fixed coefficient exceptions, $a$ can be chosen throughout an open set on the pole curve; inverse solutions based at these different $a$ give different initial values at a nearby ordinary point. These are [movable singularities of a complex differential equation](../../../../../movable-singularity-of-a-complex-differential-equation.md), contradicting the hypothesis. Hence the denominator has no genuine $w$-dependent factor: $A$ is a [polynomial](../../../../../polynomial-split.md) in $w$, with [rational functions](../../../../../rational-function.md) of $z$ as coefficients.

Let its degree in $w$ be $d$. Use the dependent coordinate $v=1/w$ on the [Riemann sphere](../../../../../riemann-sphere.md). Its equation is

$$
v'=-v^2A(z,1/v).
$$

If $d\ge3$, the right-hand side has a pole of order $d-2$ at $v=0$ for generic $z$. The same inverse-equation argument gives a movable [algebraic branch point](../../../../../algebraic-branch-point.md) of order $d-1$. It follows that $d\le2$, so **the equation is Riccati**, including its linear and constant special cases:

$$
\boxed{f'=a(z)f^2+b(z)f+c(z).}
$$

The requirement about the whole dependent-variable [Riemann sphere](../../../../../riemann-sphere.md) is essential: examining only finite values would miss the branching at $f=\infty$ for degree at least three.

The [linearization of a Riccati equation](../../../../../linearization-of-a-riccati-equation.md) is particularly symmetric in the system

$$
\binom{f_1}{f_2}'=
\begin{pmatrix}b/2&c\\-a&-b/2\end{pmatrix}
\binom{f_1}{f_2}.
$$

On a simply connected domain where the coefficients are [holomorphic](../../../../../complex-differentiability-at-a-point.md), its solutions are [holomorphic](../../../../../complex-differentiability-at-a-point.md). Direct differentiation gives

$$
\left(\frac{f_1}{f_2}\right)'=
\frac{(bf_1/2+cf_2)f_2-f_1(-af_1-bf_2/2)}{f_2^2}
=a\left(\frac{f_1}{f_2}\right)^2+b\frac{f_1}{f_2}+c.
$$

A nonzero initial vector never becomes the zero vector, by uniqueness for the [linear differential equation](../../../../../linear-differential-equation.md), so the quotient is [meromorphic](../../../../../meromorphic-function.md). Choosing initial vector $(f(z_0),1)$ represents every finite initial value, and $(1,0)$ represents infinity. At fixed coefficient singularities, a single globally [holomorphic](../../../../../complex-differentiability-at-a-point.md) vector solution need not exist; the assertion is local on ordinary domains, or on their appropriate continuation surface.

Finally, for any two finite solutions $u,v$ of the [Riccati equation](../../../../../riccati-equation.md),

$$
(u-v)'=(a(u+v)+b)(u-v).
$$

Use this identity on the four differences in

$$
K=\frac{(f-g)(h-j)}{(f-j)(h-g)}.
$$

The [logarithmic derivative](../../../../../logarithmic-derivative.md) of this [cross-ratio](../../../../../cross-ratio.md) is

$$
a(f+g+h+j-f-j-h-g)+b+b-b-b=0.
$$

Thus $K$ is constant wherever the expression is initially defined, and the identity extends as an identity of [meromorphic functions](../../../../../meromorphic-function.md). Distinctness of $g,h,j$ is preserved at ordinary points by uniqueness, interpreted on the [Riemann sphere](../../../../../riemann-sphere.md). Solving the constant [cross-ratio](../../../../../cross-ratio.md) equation gives the [Riccati cross-ratio superposition](../../../../../riccati-cross-ratio-superposition.md)

$$
\boxed{f=\frac{K(h-g)j-(h-j)g}{K(h-g)-(h-j)}.}
$$

For $K=\infty$ this means $f=j$; $K=0$ gives $g$, and $K=1$ gives $h$. The constant is selected by the initial value of $f$, so the formula represents every solution, with its denominator zeros interpreted as [poles](../../../../../pole.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
