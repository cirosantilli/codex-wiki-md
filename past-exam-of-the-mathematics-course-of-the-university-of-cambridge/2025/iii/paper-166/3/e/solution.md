<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

It is enough to prove the result for $0<\kappa<1$, since a construction for a smaller positive value gives the weaker vanishing requirement for any larger one. Apply part (b) with $\kappa/2$. For large $n$, part (c) gives linearly independent polynomials $P_0,Q_0$, and

$$
G(X,Y)=P_0(X)+YQ_0(X)
$$

satisfies $H(G)\leq C_1^n$ and has order at least

$$
\frac{(2-\kappa/2)n}{d}-2
$$

at $X=\alpha$ after setting $Y=\alpha$.

Set $\delta=\kappa/(4d)$. By the [rational multiplicity bound for a linear auxiliary polynomial](../../../../../../rational-multiplicity-bound-for-a-linear-auxiliary-polynomial.md), once $q_1$ is sufficiently large, the one-variable polynomial $G(X,y)$ has multiplicity at most $\delta n+1$ at $p_1/q_1$. Consequently there is some integer $j\leq\delta n+1$ such that

$$
D_j^XG(p_1/q_1,y)\ne0.
$$

Put $F=D_j^XG$. The [normalized derivative of a polynomial](../../../../../../normalized-derivative-of-a-polynomial.md) preserves integral coefficients and multiplies height by at most $2^n$, so $H(F)\leq C_2^n$. Differentiation lowers the vanishing order at $(\alpha,\alpha)$ by at most $j$; for sufficiently large $n$,

$$
\frac{(2-\kappa/2)n}{d}-2-j
\geq\frac{(2-\kappa)n}{d}.
$$

Finally write $F=P-YQ$ by replacing the coefficient of $Y$ by its negative. Then $F(p_1/q_1,y)\ne0$ and all the claimed bounds hold.

## ↑ Ancestors (11)

1. [E](../e.md)
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
