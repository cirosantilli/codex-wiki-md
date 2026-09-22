<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the coefficient $2-\alpha$ in the numerator, as verified in the PDF; the converted TeX lost its $-\alpha$. Multiplying the method by $2+\alpha$ gives the [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md)

$$
\rho(\zeta)=(2+\alpha)\zeta^2-4\zeta+(2-\alpha),\qquad
\sigma(\zeta)=\zeta^2+2\alpha\zeta-1.
$$

For every admissible real $\alpha$, $\rho(1)=0$ and $\rho'(1)=2\alpha=\sigma(1)$, giving [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md). Factorization gives

$$
\rho(\zeta)=(\zeta-1)\bigl((2+\alpha)\zeta-(2-\alpha)\bigr).
$$

The second root is $r=(2-\alpha)/(2+\alpha)$. The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) requires $|r|\leq1$ and forbids a repeated root at one. For real $\alpha\ne-2$,

$$
|r|\leq1\iff(2-\alpha)^2\leq(2+\alpha)^2\iff\alpha\geq0.
$$

At $\alpha=0$ both roots equal one, violating [zero-stability](../../../../../../zero-stability.md). For $\alpha>0$ the second root lies strictly inside the unit disk. The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) therefore gives

$$
\boxed{\text{convergence exactly for }\alpha>0.}
$$

To find the order rather than only consistency, expand the exact-solution residual through the generating function:

$$
\rho(e^z)-z\sigma(e^z)
=\frac\alpha3z^3+\left(\frac\alpha3-\frac16\right)z^4+O(z^5).
$$

Thus its unnormalized [local truncation error](../../../../../../local-truncation-error.md) begins with $(\alpha/3)h^3y^{(3)}$ when $\alpha>0$, and the global method order is exactly two for every convergent parameter. For comparison, $\alpha=0$ has formal order three but is not convergent because of its double unit root:

$$
\boxed{p=2\quad\text{for every }\alpha>0.}
$$

These orders assume a smooth solution, the usual local Lipschitz condition and starting approximations of the required accuracy.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
