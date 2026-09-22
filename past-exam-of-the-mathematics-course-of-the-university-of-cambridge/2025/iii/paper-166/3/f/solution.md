<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

If $\alpha$ is nonreal, its positive distance from $\mathbb R$ makes the assertion immediate, so assume $\alpha\in\mathbb R$. Fix $\varepsilon>0$ and put

$$
\mu=\frac d2+1+\varepsilon.
$$

Choose $\kappa>0$ so small that

$$
\eta:=\frac{(\mu-1)(2-\kappa)}d-1>0.
$$

Suppose for a contradiction that infinitely many reduced fractions satisfy $|\alpha-p/q|<q^{-\mu}$. Their denominators are unbounded.

Choose one such $p_1/q_1$ with $q_1$ arbitrarily large, and then a later one $p_2/q_2$ with $q_2$ arbitrarily large. Choose the integer $n$ so that

$$
q_1^{(2-\kappa)n/d}
\leq q_2
<q_1^{(2-\kappa)(n+1)/d}.
$$

Then $n$ can be made sufficiently large for part (e). Apply it with $y=p_2/q_2$. Since $F$ has integral coefficients, degree at most $n$ in $X$, and degree at most one in $Y$, its nonzero rational value satisfies the denominator bound

$$
|F(p_1/q_1,p_2/q_2)|\geq q_1^{-n}q_2^{-1}.
$$

The supplied upper estimate and the two approximation inequalities give, with $a=(2-\kappa)n/d$,

$$
|F(p_1/q_1,p_2/q_2)|
<C_3^n(q_1^{-\mu a}+q_2^{-\mu})
\leq2C_3^nq_1^{-\mu a}.
$$

Using the upper bound $q_2<q_1^{a+(2-\kappa)/d}$ in the denominator estimate and comparing yields

$$
q_1^{(\mu-1)a-n-(2-\kappa)/d}<2C_3^n.
$$

After taking $n$th roots and letting the choice of $q_2$ make $n$ large, this bounds $q_1^\eta$ by a constant depending only on $\alpha,\kappa$. That contradicts the ability to choose $q_1$ arbitrarily large. Hence only finitely many such rational approximations exist. This is the [Thue-Siegel rational approximation bound](../../../../../../thue-siegel-rational-approximation-bound.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
