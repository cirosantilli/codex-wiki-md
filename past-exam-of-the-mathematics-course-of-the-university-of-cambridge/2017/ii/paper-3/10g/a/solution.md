<h1 id="10g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $p_{-2}=0,p_{-1}=1,q_{-2}=1,q_{-1}=0$ and define the [continued fraction convergents](../../../../../../continued-fraction-convergent.md) by

$$
 p_n=a_np_{n-1}+p_{n-2},\qquad q_n=a_nq_{n-1}+q_{n-2},\qquad
 \frac{p_n}{q_n}=[a_0;\ldots,a_n].
$$

The recurrence reverses the sign of $p_nq_{n-1}-p_{n-1}q_n$, whose initial value at $n=0$ is $-1$. Hence $p_nq_{n-1}-p_{n-1}q_n=(-1)^{n-1}$. Every common [divisor](../../../../../../divisor.md) of $p_n,q_n$ divides this number, proving $\boxed{\gcd(p_n,q_n)=1}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10G](../../10g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
