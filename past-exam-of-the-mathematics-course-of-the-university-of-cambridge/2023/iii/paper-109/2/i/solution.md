<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the [Harris-Kleitman inequality](../../../../../../harris-inequality.md) by induction on $n$. For up-sets $\mathcal A,\mathcal B\subseteq\mathcal P([n])$, let $\mathcal A_0,\mathcal A_1$ be their sections according as $n$ is absent or present, and write $a_i=|\mathcal A_i|$; define $b_i$ and $c_i=|\mathcal A_i\cap\mathcal B_i|$ similarly. Monotonicity gives $a_0\leq a_1$ and $b_0\leq b_1$. The induction hypothesis on $[n-1]$ gives

$$
2^{n-1}c_i\geq a_ib_i
\qquad(i=0,1).
$$

It remains only to observe that

$$
2(a_0b_0+a_1b_1)-(a_0+a_1)(b_0+b_1)
=(a_1-a_0)(b_1-b_0)\geq0.
$$

Hence

$$
2^n|\mathcal A\cap\mathcal B|
\geq|\mathcal A|\,|\mathcal B|.
$$

The case $n=0$ starts the induction, so this is a proof from first principles.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
