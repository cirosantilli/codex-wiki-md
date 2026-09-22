<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

At a regular constrained extremal, the first variations satisfy $\delta I=\lambda\delta J$ for a constant [Lagrange multiplier](../../../../lagrange-multiplier.md) $\lambda$. One way to justify this is to choose a variation for which $\delta J\neq0$, use it to correct any other variation to preserve the constraint by the [implicit function theorem](../../../../implicit-function-theorem.md), and differentiate $I$ along that corrected family. This gives the same ratio $\lambda$ for all variations. The exceptional case $\delta J=0$ for every variation requires the usual separate abnormal-extremal analysis.

Set $L=F-\lambda G$. Integration by parts in its [first variation](../../../../first-variation.md) gives

$$
\delta(I-\lambda J)
=\left[L_{y'}\eta\right]_a^b+
\int_a^b\left(L_y-\frac d{dx}L_{y'}\right)\eta\,dx.
$$

Taking compactly supported variations and applying the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) yields the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md). For the quadratic integrands, it is

$$
\boxed{(py')'+(q+\lambda r)y=0,}
$$

or $\mathcal Ly=\lambda ry$ with $\mathcal L y=-(py')'-qy$. If endpoint values are free, independent endpoint variations give the natural conditions

$$
\boxed{p(a)y'(a)=p(b)y'(b)=0.}
$$

At a prescribed endpoint the variation instead vanishes and no natural condition is added there.

Under these natural conditions, integration by parts gives

$$
2I=\int_a^b(py'^2-qy^2)\,dx
=[py'y]_a^b+\int_a^by\mathcal Ly\,dx
=\lambda\int_a^bry^2\,dx=2\lambda J.
$$

Hence $\boxed{I=\lambda J}$. For two solutions satisfying the same natural conditions, subtract their cross-multiplied equations and integrate:

$$
(\lambda_m-\lambda_n)\int_a^bry_my_n\,dx
=\int_a^b(y_n\mathcal Ly_m-y_m\mathcal Ly_n)\,dx=0.
$$

The final equality is the vanishing endpoint boundary form. Thus distinct [eigenvalues](../../../../eigenvalue.md) give

$$
\boxed{\int_a^b r y_m y_n\,dx=0.}
$$

The same argument works for other common homogeneous boundary conditions making that boundary form zero.

In the Legendre case, $((1-x^2)y_n')'+\lambda_ny_n=0$. Comparing coefficients of $x^n$ in a degree-$n$ solution gives $\lambda_n=n(n+1)$, so different degrees have different [eigenvalues](../../../../eigenvalue.md). A degree-zero solution is $y_0=C_0$. A linear solution $Ax+B$ must be orthogonal to the nonzero constant solution, so $B=0$ and $y_1=C_1x$. Write $y_2=Ax^2+Bx+C$. [Orthogonality](../../../../orthogonal-vectors.md) to $x$ gives $B=0$, and [orthogonality](../../../../orthogonal-vectors.md) to $1$ gives $2A/3+2C=0$. Therefore

$$
\boxed{y_2=C_2\frac{3x^2-1}{2}.}
$$

The constants are free [normalization](../../../../normalization.md) factors; for solutions of the stated exact degrees they are nonzero. The natural endpoint conditions hold automatically for these [polynomials](../../../../polynomial-split.md) because $p(\pm1)=0$.

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
