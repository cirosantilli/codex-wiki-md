<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

[Ordinal exponentiation](../../../../../ordinal-exponentiation.md) is defined by

$$
\omega^0=1,
\qquad
\omega^{\beta+1}=\omega^\beta\omega,
\qquad
\omega^\lambda=\sup_{\beta<\lambda}\omega^\beta
$$

for limit $\lambda$. [Transfinite induction](../../../../../transfinite-induction.md) gives $\omega^\alpha\geq\alpha$. Since $\omega^{\alpha+1}>\alpha$, there is a least $\alpha^*$ with $\omega^{\alpha^*}>\alpha$. If nonzero $\alpha^*$ were a limit, the defining supremum would imply $\omega^\beta>\alpha$ for some $\beta<\alpha^*$, a contradiction. Hence $\alpha^*$ is a successor.

For $\alpha>0$, write $\alpha^*=\beta+1$. Then $\omega^\beta\leq\alpha<\omega^{\beta+1}$. There is a largest positive integer $n$ with $\omega^\beta n\leq\alpha$, and ordinal division gives

$$
\alpha=\omega^\beta n+\gamma,
\qquad
\gamma<\omega^\beta.
$$

Repeating on $\gamma$ terminates because there is no infinite strictly decreasing sequence of ordinals, producing the [Cantor normal form](../../../../../cantor-normal-form.md)

$$
\alpha=\omega^{\beta_1}n_1+\cdots+\omega^{\beta_k}n_k,
\qquad
\beta_1>\cdots>\beta_k.
$$

For two monomials,

$$
\omega^{\delta_1}m_1+\omega^{\delta_2}m_2=
\begin{cases}
\omega^{\delta_2}m_2,&\delta_1<\delta_2,\\
\omega^{\delta_1}(m_1+m_2),&\delta_1=\delta_2,\\
\omega^{\delta_1}m_1+\omega^{\delta_2}m_2,&\delta_1>\delta_2.
\end{cases}
$$

For general $\alpha+\alpha'$, compare the leading exponent $\beta'_1$ with the exponents of $\alpha$: discard every trailing term of $\alpha$ having exponent below $\beta'_1$, combine coefficients if the last retained exponent equals $\beta'_1$, and then append all remaining terms of $\alpha'$. This is its Cantor normal form.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
