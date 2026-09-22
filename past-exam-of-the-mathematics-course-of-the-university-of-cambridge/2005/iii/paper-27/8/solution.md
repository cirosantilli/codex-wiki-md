<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Fix an [ordinal](../../../../../ordinal.md) $\rho>1$. The [Generalized Cantor normal form](../../../../../generalized-cantor-normal-form.md) asserts that every nonzero ordinal $\alpha$ has a unique expression

$$
\boxed{\alpha=\rho^{\beta_0}\xi_0+\rho^{\beta_1}\xi_1+\cdots+\rho^{\beta_{m-1}}\xi_{m-1}},
\qquad
\beta_0>\beta_1>\cdots>\beta_{m-1},\quad0<\xi_i<\rho.
$$

Products, sums and powers here are [ordinal multiplication](../../../../../ordinal-multiplication.md), [ordinal addition](../../../../../ordinal-addition.md) and [ordinal exponentiation](../../../../../ordinal-exponentiation.md); the coefficients need not be finite if $\rho$ is infinite. The case $\rho=\omega$ is [Cantor normal form](../../../../../cantor-normal-form.md), and a finite base on finite ordinals gives ordinary positional notation. Zero has the empty expansion.

We first prove the [ordinal division algorithm](../../../../../ordinal-division-algorithm.md). For $\delta>0$, the function $q\mapsto\delta q$ is strictly increasing, continuous at limit ordinals and unbounded. Hence there is a greatest $q$ with $\delta q\le\alpha$: the first $q'$ with $\delta q'>\alpha$ cannot be a limit by continuity and must equal $q+1$. The interval after the initial segment $\delta q$ has a unique order type $r$, so $\alpha=\delta q+r$. Maximality of $q$ gives $r<\delta$. These facts also prove uniqueness of $q,r$.

Similarly $\beta\mapsto\rho^\beta$ is strictly increasing, continuous at limits and unbounded, so there is a unique largest $\beta_0$ with $\rho^{\beta_0}\le\alpha$. Divide by $\rho^{\beta_0}$ to obtain

$$
\alpha=\rho^{\beta_0}\xi_0+r_0,\qquad r_0<\rho^{\beta_0}.
$$

The quotient is positive, and $\alpha<\rho^{\beta_0+1}=\rho^{\beta_0}\rho$ makes $\xi_0<\rho$. If $r_0>0$, repeat on $r_0$; its leading exponent is strictly smaller than $\beta_0$. This process terminates, since an infinite run would give an infinite descending sequence of ordinals. It constructs the required form.

For uniqueness, a finite expression with largest exponent $\beta$ and coefficients below $\rho$ has value below $\rho^{\beta+1}$. Prove this from the end backwards: a tail with largest exponent $\gamma<\beta$ is below $\rho^{\gamma+1}\le\rho^\beta$, and

$$
\rho^\beta\xi+\text{tail}<\rho^\beta(\xi+1)\le\rho^\beta\rho.
$$

Thus the displayed leading exponent is the uniquely determined largest $\beta$ with $\rho^\beta\le\alpha$. The [ordinal division algorithm](../../../../../ordinal-division-algorithm.md) uniquely determines its coefficient and the remaining tail, and recursion proves uniqueness of the whole expression. No commutative rearrangement of ordinal sums is used.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
