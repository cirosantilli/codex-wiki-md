<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

The recursive [ordinal addition](../../../../../ordinal-addition.md) definitions are $a+0=a$, $a+(b+1)=(a+b)+1$, and $a+\lambda=\sup_{b<\lambda}(a+b)$ for a nonzero limit [ordinal](../../../../../ordinal.md). [Ordinal multiplication](../../../../../ordinal-multiplication.md) is $a\cdot0=0$, $a\cdot(b+1)=a\cdot b+a$, and $a\cdot\lambda=\sup_{b<\lambda}a\cdot b$. For $a>0$, [ordinal exponentiation](../../../../../ordinal-exponentiation.md) is $a^0=1$, $a^{b+1}=a^b\cdot a$, and $a^\lambda=\sup_{b<\lambda}a^b$; the exceptional zero base has $0^0=1$ and $0^b=0$ for $b>0$.

Transfinite induction gives $\omega^a\geq a$. At zero this is immediate; at a successor, $\omega^{b+1}=\omega^b\omega\geq\omega^b+1\geq b+1$. At a limit, continuity and the induction hypothesis give $\sup_{b<a}\omega^b\geq\sup_{b<a}b=a$. Also $a\mapsto\omega^a$ is strictly increasing: its successor values strictly increase, and continuity preserves the strict inequality between any two distinct indices.

For $\alpha>0$, $\omega^{\alpha+1}>\omega^\alpha\geq\alpha$, so there is a least $\delta$ with $\omega^\delta>\alpha$. It cannot be zero and cannot be a limit: at a limit, a [supremum](../../../../../supremum.md) greater than $\alpha$ has a term already greater than $\alpha$, contradicting minimality. Thus $\delta=\alpha_0+1$, and

$$
\boxed{\omega^{\alpha_0}\leq\alpha<\omega^{\alpha_0+1}.}
$$

Strict increase proves uniqueness, and $\alpha_0\leq\omega^{\alpha_0}\leq\alpha$ proves the requested index bound.

Choose the largest positive integer $a_0$ with $\omega^{\alpha_0}a_0\leq\alpha$. It exists because $\alpha<\omega^{\alpha_0}\omega=\sup_{m<\omega}\omega^{\alpha_0}m$. The remaining tail of the [ordinal](../../../../../ordinal.md) interval has an order type $\rho$ with $\alpha=\omega^{\alpha_0}a_0+\rho$; maximality implies $\rho<\omega^{\alpha_0}$. If $\rho>0$, repeat the construction on it. The leading exponents strictly decrease, and there is no infinite strictly decreasing [sequence](../../../../../sequence.md) of [ordinals](../../../../../ordinal.md): its set of values would have a least member followed by a smaller one. Hence the process terminates, yielding the [Cantor normal form](../../../../../cantor-normal-form.md)

$$
\boxed{\alpha=\omega^{\alpha_0}a_0+\omega^{\alpha_1}a_1+\cdots+\omega^{\alpha_n}a_n,
\quad\alpha_0>\cdots>\alpha_n,\quad a_j\in\mathbb N_{>0}.}
$$

The first exponent is determined by the preceding band, the first coefficient by maximality, and the tail by the [ordinal](../../../../../ordinal.md) interval left after that initial segment. Recursion therefore proves uniqueness of every exponent and coefficient. The PDF's second coefficient is printed $\alpha_1$ rather than $a_1$; the stated natural-number coefficients and the construction identify the intended expression.

For the final assertion, powers of $\omega$ are additively indecomposable: if $\tau<\omega^\eta$, then $\tau+\omega^\eta=\omega^\eta$ for $\eta>0$. One proves this by induction on $\eta$. At a successor, bound $\tau$ by a finite multiple of $\omega^{\eta-1}$ and use the [supremum](../../../../../supremum.md) over all such multiples; at a limit, bound $\tau$ by a smaller power and use continuity. For $\eta=0$ the only possible $\tau$ is zero. Thus a smaller leading exponent is absorbed when a larger-leading [ordinal](../../../../../ordinal.md) is added on its right. If $\beta,\gamma$ have unequal leading exponents, either $\beta+\gamma=\gamma$ or $\gamma+\beta=\beta$. If their leading exponents coincide, the leading coefficient of either sum is the sum of their two positive leading coefficients; it exceeds each coefficient, so neither absorption equality holds. Zero is never commensurable with an [ordinal](../../../../../ordinal.md). Consequently **commensurability is exactly equality of the leading exponent**, equivalently membership of both positive [ordinals](../../../../../ordinal.md) in one of the stated bands.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
