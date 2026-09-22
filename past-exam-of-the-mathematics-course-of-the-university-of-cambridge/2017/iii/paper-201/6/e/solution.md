<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Specify the sign convention for the [Lévy characteristic exponent](../../../../../../characteristic-exponent-of-a-levy-process.md) by

$$
\mathbb E e^{iuX_a}=e^{-a\Psi(u)}.
$$

Conditioning on $T_a$ and using the [Brownian first-passage Laplace transform](../../../../../../brownian-first-passage-laplace-transform.md) gives

$$
\mathbb E e^{iuW_{T_a}}=\mathbb E e^{-u^2T_a/2}
=e^{-a\sqrt{u^2}}=e^{-a|u|}.
$$

Therefore

$$
\boxed{\Psi(u)=|u|.}
$$

The absolute value is essential for negative $u$. The process is the standard symmetric [Cauchy process](../../../../../../cauchy-process.md); for $a>0$, $X_a$ has the [Cauchy distribution](../../../../../../cauchy-distribution.md) with location zero and scale $a$. If the exponent convention instead uses $\mathbb E e^{iuX_a}=e^{a\psi(u)}$, the answer is $\psi(u)=-|u|$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
