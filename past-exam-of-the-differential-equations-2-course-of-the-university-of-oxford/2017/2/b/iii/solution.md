<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the normalization from part (ii), and write

$$
N_k=\int_1^e r\widehat y_k^2\,dx=\frac12,\qquad
I_k=\int_1^e r\widehat y_k e^x\,dx
=\int_1^e\frac{e^x}{x^2}\sin(k\pi\log x)\,dx.
$$

The [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md) coefficient is $c_k=N_k^{-1}\int_1^e ry\widehat y_k\,dx$. Although $\widehat y_k$ has zero endpoint values, $y$ generally does not. Retain the endpoint term in the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md):

$$
\begin{aligned}
\int_1^e\bigl(\widehat y_k\widehat Ly-y\widehat L\widehat y_k\bigr)\,dx
&=\bigl[x^{-1}(\widehat y_k y'-\widehat y_k' y)\bigr]_1^e\\
&=\alpha\widehat y_k'(1)=\alpha k\pi.
\end{aligned}
$$

The positive sign comes from subtracting the contribution at $x=1$. The differential equation also gives $\widehat Ly=re^x-(\beta-1)ry$. Substitution into the preceding identity yields

$$
I_k-(\beta-1+\widehat\lambda_k)c_kN_k=\alpha k\pi.
$$

Hence, away from [resonance in a differential equation](../../../../../resonance-in-a-differential-equation.md),

$$
\boxed{c_k=\frac{2(I_k-\alpha k\pi)}{\beta-1-k^2\pi^2}
=\frac{2\left[\alpha k\pi-\int_1^e e^x x^{-2}\sin(k\pi\log x)\,dx\right]}{1+k^2\pi^2-\beta}.}
$$

This is the effect of [boundary data in a Sturm-Liouville eigenfunction expansion](../../../../../boundary-data-in-a-sturm-liouville-eigenfunction-expansion.md): omitting the endpoint contribution would discard the dependence on $\alpha$.

If $\beta=1+n^2\pi^2$ for a positive integer $n$, the [Fredholm solvability condition](../../../../../fredholm-solvability-condition.md) is

$$
\boxed{I_n=\alpha n\pi.}
$$

When it fails, there is **no solution**. When it holds, $c_n$ is arbitrary and the other coefficients retain the displayed formula, giving **infinitely many solutions** differing by a multiple of $\widehat y_n$. Sufficiency follows by subtracting the smooth lift $h(x)=\alpha x(1-\log x)$, which has the required endpoint values and satisfies $Lh=0$, and applying the [Fredholm alternative](../../../../../fredholm-alternative.md) to the resulting homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md).

Finally, for $\alpha\ne0$, the displayed [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md) represents the solution on $1<x<e$ and in the [weighted inner product](../../../../../weighted-inner-product.md) sense. Every term is zero at $x=1$, so that series cannot give the nonzero prescribed value by substitution at the endpoint. The [boundary trace](../../../../../boundary-trace-of-a-function.md) must be imposed separately. Equivalently, expand $y-h$ with homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) and add $h$ back afterwards.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
