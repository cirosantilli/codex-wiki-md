<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**No.** A necessary condition for [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) is reproduction of the constant solution $y(x)=1$ of the [ordinary differential equation](../../../../../ordinary-differential-equation.md) $y'=0$. In a [linear multistep method](../../../../../linear-multistep-method-split.md) this gives

$$
\rho(1)=\sum_{j=0}^k\alpha_j=0.
$$

But the reverse [triangle inequality](../../../../../triangle-inequality.md) gives, under the strict coefficient inequality,

$$
\boxed{|\rho(1)|\geq|\alpha_k|-\sum_{j=0}^{k-1}|\alpha_j|>0.}
$$

Thus the necessary [order conditions for a linear multistep method](../../../../../order-conditions-for-a-linear-multistep-method.md) already fail at order zero, regardless of the values of the $\beta_j$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
