<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Set

$$
p_{-2}=0, p_{-1}=1,\qquad q_{-2}=1, q_{-1}=0,
$$

and recursively

$$
p_n=a_np_{n-1}+p_{n-2},\qquad q_n=a_nq_{n-1}+q_{n-2}.
$$

Then $p_n/q_n=[a_0,ldots,a_n]$. The [determinant](../../../../../determinant.md) identity

$$
p_nq_{n-1}-p_{n-1}q_n=(-1)^{n-1}
$$

follows by induction. Writing the remaining complete quotient as $\theta_{n+1}>1$ gives

$$
\theta=\frac{p_n\theta_{n+1}+p_{n-1}}
{q_n\theta_{n+1}+q_{n-1}},
$$

so $\theta$ lies strictly between consecutive convergents and their order alternates. For odd $n$,

$$
\frac{p_{n-1}}{q_{n-1}}<\theta<\frac{p_n}{q_n}.
$$

Moreover $|\theta-p_n/q_n|<1/(q_nq_{n+1})$, and $q_n\to\infty$, proving convergence.

The continued-fraction algorithm gives

$$
\boxed{\sqrt7=[2;\overline{1,1,1,4}].}
$$

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
