<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Write the [continued fraction](../../../../../continued-fraction.md) as $\theta=[a_0;a_1,a_2,\ldots]$ and define its [convergents](../../../../../continued-fraction-convergent.md) by

$$
p_{-1}=1,\quad p_0=a_0,\quad p_n=a_np_{n-1}+p_{n-2},
$$



$$
q_{-1}=0,\quad q_0=1,\quad q_n=a_nq_{n-1}+q_{n-2}.
$$

Induction using these recurrences gives

$$
p_nq_{n-1}-p_{n-1}q_n
=-(p_{n-1}q_{n-2}-p_{n-2}q_{n-1})
=\boxed{(-1)^{n-1}}.
$$

In particular, consecutive convergents have coprime numerator and denominator. The standard best-approximation consequence of the same determinant identity is that, for $0<q\le q_n$ and $p/q\ne p_n/q_n$,

$$
|q\theta-p|>|q_n\theta-p_n|.
$$

Dividing by $q\le q_n$ gives

$$
\left|\theta-\frac pq\right|
=\frac{|q\theta-p|}{q}
>\frac{|q_n\theta-p_n|}{q_n}
=\left|\theta-\frac{p_n}{q_n}\right|.
$$

The contrapositive proves that any strictly better approximation has $q>q_n$.

For $\sqrt{12}$, the [continued-fraction algorithm](../../../../../continued-fraction-algorithm.md) gives

$$
\sqrt{12}=3+(\sqrt{12}-3),
\qquad
\frac1{\sqrt{12}-3}=2+\frac1{\sqrt{12}+3},
$$

and the remainder then repeats. Hence

$$
\boxed{\sqrt{12}=[3;\overline{2,6}]}.
$$

The convergent $[3;2]=7/2$ supplies a solution of the [Pell equation](../../../../../pell-equation.md):

$$
\boxed{x=7,\qquad y=2},
\qquad 7^2-12\cdot2^2=1.
$$

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
