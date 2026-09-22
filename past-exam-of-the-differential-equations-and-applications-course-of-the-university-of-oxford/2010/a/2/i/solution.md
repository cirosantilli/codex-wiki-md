<h1 id="a/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $t=\log x$, so $0<t<\pi$, and write $y(x)=x^{-2}w(t)$. Direct differentiation of this [Cauchy-Euler equation](../../../../../cauchy-euler-equation.md) gives

$$
x^2y''+5xy'+y=x^{-2}(w''-3w).
$$

The [eigenvalue](../../../../../eigenvalue.md) equation is therefore $-w''=(\lambda-3)w$ with $w(0)=w(\pi)=0$. For $\lambda-3\leq0$, the linear/hyperbolic solutions cannot satisfy both endpoint conditions except trivially. For $\lambda-3>0$, the sine solution vanishes at both endpoints exactly when its frequency is a positive [integer](../../../../../integer-split.md). Thus

$$
\boxed{\lambda_k=k^2+3,\qquad y_k(x)=x^{-2}\sin(k\log x),\qquad k=1,2,\ldots.}
$$

Each associated [eigenspace](../../../../../eigenspace.md) is one-dimensional.

**The displayed differential operator is not [self-adjoint](../../../../../self-adjoint-operator.md) for the unweighted [inner product](../../../../../inner-product-split.md).** Let $A=x^2\partial_x^2+5x\partial_x+1$. [Integration by parts](../../../../../integration-by-parts.md) on compactly supported smooth functions gives its [formal adjoint](../../../../../formal-adjoint.md)

$$
A^*f=(x^2f)''-(5xf)'+f=x^2f''-xf'-2f,
$$

which differs from $A$. One can see an explicit failure of symmetry without boundary terms: take a nonzero real compactly supported smooth $f$ in the interval and $g=xf$. Then

$$
\langle f,Ag\rangle-\langle Af,g\rangle=3\int_1^{e^\pi}x(fg'-f'g)\,dx=3\int_1^{e^\pi}xf^2\,dx>0.
$$

Both [test functions](../../../../../test-function.md) obey the Dirichlet endpoint conditions. Changing the sign of $A$ for the eigenproblem does not repair this failure. A different, weighted [inner product](../../../../../inner-product-split.md) with weight $x^3$ does give the [Sturm-Liouville form](../../../../../sturm-liouville-form.md) $x^3Ay=(x^5y')'+x^3y$, explaining why a real discrete [spectrum](../../../../../spectrum-functional-analysis.md) is nevertheless natural.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
