<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the operator in divergence form:

$$
\mathcal Ly=\big((1-x^2)y'\big)'.
$$

The [Legendre differential equation](../../../../../legendre-differential-equation.md) therefore gives

$$
\boxed{\mathcal LP_n=-n(n+1)P_n,\qquad n=0,1,2,\ldots}.
$$

These are the [eigenvalues](../../../../../eigenvalue.md) of $\mathcal L$. With the common positive-sign convention for a [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md), use $-\mathcal L$ instead:

$$
-\big(pP_n'\big)'=\lambda_n wP_n,\qquad
\boxed{p=1-x^2,\quad q=0,\quad w=1,\quad\lambda_n=n(n+1)}.
$$

This is a singular [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md), because $p$ vanishes at the endpoints. Bounded [eigenfunctions](../../../../../eigenfunction.md) select the nonlogarithmic branches and satisfy $pP_n'\to0$ there. The [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md) gives

$$
[m(m+1)-n(n+1)]\int_{-1}^1P_mP_n\,dx
=[(1-x^2)(P_mP_n'-P_nP_m')]_{-1}^1=0.
$$

The [eigenvalues](../../../../../eigenvalue.md) are distinct, proving the [orthogonality](../../../../../orthogonal-vectors.md) condition

$$
\boxed{\int_{-1}^1P_m(x)P_n(x)\,dx=0\quad(m\ne n)}.
$$

The weight is one. No choice of normalization of the [Legendre polynomials](../../../../../legendre-polynomial.md) is needed for this conclusion.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
