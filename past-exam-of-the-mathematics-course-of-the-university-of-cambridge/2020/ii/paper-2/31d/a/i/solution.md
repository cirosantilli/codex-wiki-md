<h1 id="31d/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fixed $n$, define the remainders

$$
r_n=f-\sum_{j=0}^na_j\phi_j,
\qquad
r_{n+1}=f-\sum_{j=0}^{n+1}a_j\phi_j.
$$

The hypotheses say $r_n=o(\phi_n)$ and $r_{n+1}=o(\phi_{n+1})$, while subtraction gives

$$
r_n=a_{n+1}\phi_{n+1}+r_{n+1}.
$$

Because $a_{n+1}\ne0$,

$$
\frac{r_n}{\phi_{n+1}}\longrightarrow a_{n+1}.
$$

For $x$ sufficiently close to $x_0$ this denominator is therefore nonzero, and

$$
\frac{\phi_{n+1}}{\phi_n}
=\frac{r_n/\phi_n}{r_n/\phi_{n+1}}
\longrightarrow\frac0{a_{n+1}}=0.
$$

**Thus $\phi_{n+1}=o(\phi_n)$ for every $n$, so $(\phi_n)$ is an [asymptotic sequence](../../../../../../../asymptotic-sequence.md).**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [31D](../../../31d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
