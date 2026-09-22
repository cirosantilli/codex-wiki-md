<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first characteristic [polynomial](../../../../../polynomial-split.md) factors as

$$
\rho(\zeta)=\zeta^3+\alpha\zeta^2-\alpha\zeta-1
=(\zeta-1)[\zeta^2+(\alpha+1)\zeta+1].
$$

The two quadratic roots have product one. Both can lie in the closed unit disk only if both have modulus one, requiring $|\alpha+1|\leq2$. At $\alpha=-3$ the root one is triple and $\beta=0$; at $\alpha=1$ the root minus one is double. Both fail the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md). In the intervening open interval the two quadratic roots are distinct conjugate unit-modulus roots, different from one. Thus

$$
\boxed{-3<\alpha<1\quad\text{is exactly the zero-stability range}.}
$$

Using $2\beta=\alpha+3$, the supplied expansion gives

$$
C_0=C_1=C_2=0,\qquad C_3=\frac{9-\alpha}{12},\qquad
C_4=\frac{9-\alpha}{8},\qquad C_5=\frac{231-23\alpha}{240}.
$$

Throughout the [zero-stable](../../../../../zero-stability.md) range, $C_3\ne0$, so **every such method has order two**. There is a unique higher-order choice:

$$
\boxed{\alpha=9,\qquad\beta=6.}
$$

Here $C_3=C_4=0$ and $C_5=1/10\ne0$, giving exactly order four, with normalized leading truncation error $h^4y^{(5)}/120$. But the extra roots are $-5\pm2\sqrt6$, one of modulus greater than one. By the [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) this consistent but non-[zero-stable](../../../../../zero-stability.md) method is **not convergent** for arbitrary consistent starting values.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
