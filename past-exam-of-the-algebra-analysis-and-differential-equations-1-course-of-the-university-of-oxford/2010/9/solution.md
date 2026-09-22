<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

For $p$ in a half-plane of absolute convergence, interchange the integrals using [Fubini's theorem](../../../fubini-s-theorem.md):

$$
\overline g(p)=\int_0^\infty f(s)\int_s^\infty e^{-pt}dt\,ds
=\boxed{\overline f(p)/p.}
$$

For positive real $p$, integration by parts gives $I_n=\int_0^\infty e^{-pt}t^n dt=nI_{n-1}/p$, starting from $I_0=1/p$. Hence $I_n=n!/p^{n+1}$, or

$$
\boxed{\mathcal L(t^n/n!)(p)=p^{-n-1}.}
$$

The formula extends throughout $\operatorname{Re}p>0$ by the same integration argument. Write $X=\mathcal Lx$. The integral term is the [convolution](../../../convolution.md) of $t$ with $x(t)$, whose [Laplace transform](../../../laplace-transform.md) is $X/p^2$. The derivative transforms to $pX-x(0)=pX-1$. Therefore

$$
(p+p^{-2})X-1=p^{-2}+p^{-3}+p^{-5},
$$

and elementary factorization gives

$$
X=\frac{p^5+p^3+p^2+1}{p^3(p^3+1)}
=\frac{(p^2+1)(p^3+1)}{p^3(p^3+1)}
=\frac1p+\frac1{p^3}.
$$

Inverting the two polynomial transforms yields

$$
\boxed{x(t)=1+\tfrac12t^2.}
$$

Direct substitution verifies $x'=t$ and $\int_0^t(t-s)(1+s^2/2)ds=t^2/2+t^4/24$, as required. Uniqueness also follows without transform assumptions: differentiating the equation twice gives $x^{(3)}+x=1+t^2/2$ with initial data $x(0)=1$, $x'(0)=0$, $x''(0)=1$, a linear initial-value problem with a unique solution.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2010](../../2010-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
