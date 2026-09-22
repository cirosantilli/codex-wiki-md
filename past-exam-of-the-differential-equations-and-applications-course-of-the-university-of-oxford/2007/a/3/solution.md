<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Multiplication by an [integrating factor](../../../../integrating-factor.md) gives

$$
\boxed{p(x)=\exp\!\left(\int^xa(s)\,ds\right),\quad r=pc,\quad q=-pb,}
$$

since $p'=ap$ and hence $(pw')'=p(w''+aw')$.

For the singular-endpoint equation, take $p=x^{-1/2}$, $r=x^{1/2}/2$, $q=0$. The [indicial equation](../../../../indicial-equation.md) is $\alpha(2\alpha-3)=0$. The constant branch violates the zero endpoint value unless its coefficient vanishes; the nontrivial admissible branch therefore has $\boxed{\alpha=3/2}$. More precisely, an [eigenfunction](../../../../eigenfunction.md) has $w=Cx^{3/2}+O(x^{9/2})$ and $w'=(3C/2)x^{1/2}+O(x^{7/2})$ near zero.

Integrate the [self-adjoint](../../../../self-adjoint-operator.md) equation after multiplying by $w$, initially on $[a,1]$ with $a>0$:

$$
[wx^{-1/2}w']_a^1-\int_a^1x^{-1/2}(w')^2\,dx
+\frac\lambda2\int_a^1x^{1/2}w^2\,dx=0.
$$

At zero the boundary expression is $O(x^{3/2})$, the first [integrand](../../../../integrand.md) is $O(x^{1/2})$, and the second is $O(x^{7/2})$. Both [integrals](../../../../integral-split.md) converge and the [boundary term](../../../../boundary-term.md) vanishes. Division by the positive [weighted norm](../../../../weighted-norm.md) gives $\boxed{\lambda=I(w)}$.

The change of coordinate $z=x^{3/2}$, $w(x)=W(z)$ gives exactly

$$
W''+\frac{2\lambda}{9}W=0,\qquad W(0)=W(1)=0.
$$

Thus $\lambda_n=9n^2\pi^2/2$ and $w_n=\sin(n\pi x^{3/2})$. To prove a minimum over trial functions, rather than just identify the least [eigenvalue](../../../../eigenvalue.md), transform the quotient itself:

$$
I(w)=\frac92\frac{\int_0^1(W')^2\,dz}{\int_0^1W^2\,dz}\geq\boxed{\frac{9\pi^2}2}.
$$

The Dirichlet [Poincaré inequality](../../../../poincare-inequality.md) gives the last step, with equality precisely for a nonzero multiple of $W=\sin\pi z$. The trial class is the nonzero finite-energy class with zero [Sobolev traces](../../../../trace-operator.md); endpoint values alone without an integrability requirement do not define a finite quotient. This is the [Power-coordinate reduction of a singular Sturm-Liouville quotient](../../../../power-coordinate-reduction-of-a-singular-sturm-liouville-quotient.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the differential equations and applications course of the University of Oxford](../../../split.md)
5. [Differential equations and applications course of the University of Oxford](../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
