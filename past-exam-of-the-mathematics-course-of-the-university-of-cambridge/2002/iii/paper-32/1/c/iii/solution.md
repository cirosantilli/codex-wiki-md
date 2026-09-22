<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

When the two factor-exposure rows are [independent](../../../../../../../independent-random-variables.md), every three-column excess-coefficient matrix being singular means that the entire coefficient matrix has [rank](../../../../../../../rank-one-quadratic-form.md) at most two. The constant excess-return row must therefore be in the span of the two exposure rows. There are common constants $\theta_1,\theta_2$ such that

$$
a_i-R=\theta_1b_i+\theta_2c_i\quad\text{for every }i.
$$

To see that the constants are common, fix two assets with [independent](../../../../../../../independent-random-variables.md) exposure columns, solve their two equations for $\theta_1,\theta_2$, and apply the zero [determinant](../../../../../../../determinant.md) with any third asset; its constant entry is forced to satisfy the same equation. Taking [expectations](../../../../../../../expected-value.md) gives the exact two-factor [arbitrage pricing theory](../../../../../../../arbitrage-pricing-theory.md) formula

$$
\boxed{\mathbb E r_i=R+b_i\lambda_1+c_i\lambda_2,\qquad
\lambda_1=\theta_1+\mathbb E f_1,\quad\lambda_2=\theta_2+\mathbb E f_2.}
$$

An asset with unit loading on one factor and zero loading on the other has excess [expected return](../../../../../../../expected-return.md) equal to that factor's premium. This recovers part (i).

The [rank](../../../../../../../rank-one-quadratic-form.md) qualification matters: singularity by itself would not identify two premiums if both exposure rows were dependent. More generally, write the exposure matrix as $B$. A position $v\in\ker B$ has a constant excess payoff $(a-R\mathbf1)^tv$. Absence of [arbitrage](../../../../../../../arbitrage.md) forces this constant to vanish, so $a-R\mathbf1$ annihilates $\ker B$ and belongs to the [row space](../../../../../../../row-space.md) of $B$. This proves [exact factor pricing without idiosyncratic risk](../../../../../../../exact-factor-pricing-without-idiosyncratic-risk.md) also in a reduced-rank model, though factor premiums need not then be unique. Independence of the random factors is not a substitute for their being spanned by traded exposures.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
