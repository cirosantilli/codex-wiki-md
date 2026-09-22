<h1 id="11g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set

$$
p_{-2}=0,\qquad p_{-1}=1,\qquad
q_{-2}=1,\qquad q_{-1}=0,
$$

and for $n\geq0$ define

$$
p_n=a_np_{n-1}+p_{n-2},
\qquad
q_n=a_nq_{n-1}+q_{n-2}.
$$

Then $p_n/q_n=[a_0,\ldots,a_n]$ is the $n$th convergent.

For a variable final tail $x$, induction on $n$, or multiplication of the continued-fraction matrices, gives

$$
[a_0,\ldots,a_n,x]
=\frac{p_nx+p_{n-1}}{q_nx+q_{n-1}}.
$$

Indeed, the identity is immediate for $n=0$, and replacing the tail by $a_{n+1}+1/x$ gives the recurrence above. Taking $x=\gamma>0$ proves the formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11G](../../11g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
