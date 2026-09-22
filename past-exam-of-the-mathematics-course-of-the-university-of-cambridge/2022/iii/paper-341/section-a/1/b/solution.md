<h1 id="section-a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $s=1$, imposing order two gives

$$
\rho_0=-1,
\qquad \sigma_0=\sigma_1=\frac12.
$$

The method is therefore the [trapezoidal rule](../../../../../../../trapezoidal-rule.md)

$$
y_{n+1}-y_n=\frac h2(f_{n+1}+f_n).
$$

Its first [characteristic polynomial](../../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) is $\rho(\zeta)=\zeta-1$, so it satisfies the [root condition for a multistep method](../../../../../../../root-condition-for-a-multistep-method.md).

For $s=2$, the four conditions through order three give

$$
\rho_0=-\frac15,
\qquad \rho_1=-\frac45,
\qquad \sigma_1=\frac45,
\qquad \sigma_2=\frac25,
$$

and hence

$$
y_{n+2}-\frac45y_{n+1}-\frac15y_n
=h\left(\frac25f_{n+2}+\frac45f_{n+1}\right).
$$

Here

$$
\rho(\zeta)=\zeta^2-\frac45\zeta-\frac15
=(\zeta-1)\left(\zeta+\frac15\right),
$$

so the [root condition for a multistep method](../../../../../../../root-condition-for-a-multistep-method.md) again holds. Both methods are consistent and zero-stable, and the [Dahlquist equivalence theorem](../../../../../../../dahlquist-equivalence-theorem.md) therefore proves that both are convergent.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Section A](../../../section-a.md)
4. [Paper 341](../../../../paper-341-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
