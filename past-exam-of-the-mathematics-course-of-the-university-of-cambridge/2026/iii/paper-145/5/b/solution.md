<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write each hyperplane as $h_j(x)=0$, normalized so that $h_j(0)=1$, and put

$$
P(x)=\prod_{j=1}^m h_j(x).
$$

Then $P(0)=1$ and $P$ vanishes at every other point of $\mathbb F_q^n$. Reduce $P$ modulo $x_i^q-x_i$ in every variable. This preserves its function on $\mathbb F_q^n$, does not increase total degree, and gives the unique representative with each variable degree at most $q-1$.

The unique reduced polynomial for the delta function at zero is

$$
\prod_{i=1}^n(1-x_i^{q-1}),
$$

whose total degree is $(q-1)n$. Hence

$$
m=\deg P\geq(q-1)n.
$$

Uniqueness follows equally from the Alon-Tarsi lemma on the grids $A_i=\mathbb F_q$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 145](../../../paper-145-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
