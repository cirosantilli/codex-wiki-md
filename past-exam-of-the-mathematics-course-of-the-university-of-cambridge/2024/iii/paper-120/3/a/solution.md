<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under the [Implicational Curry-Howard correspondence](../../../../../../implicational-curry-howard-correspondence.md), propositions are simple types and assumptions are typed variables. The natural-deduction rules

$$
\frac{\Gamma,A\vdash B}{\Gamma\vdash A\to B}
\qquad\text{and}\qquad
\frac{\Gamma\vdash A\to B\quad\Gamma\vdash A}{\Gamma\vdash B}
$$

correspond respectively to the typing rules

$$
\frac{\Gamma,x:A\vdash M:B}{\Gamma\vdash\lambda x.M:A\to B},
\qquad
\frac{\Gamma\vdash M:A\to B\quad\Gamma\vdash N:A}{\Gamma\vdash MN:B}.
$$

An assumption $x:A$ corresponds to the variable rule. Induction on a proof converts each rule into the matching typing construction; induction on a typing derivation reverses the process. Thus derivability of an implicational formula from assumptions is equivalent to inhabitation of its corresponding type.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
