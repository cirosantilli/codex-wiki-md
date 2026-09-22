<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix an effective syntax encoding for the language. Let $E_s$ be the finite set of axioms observed in the first $s$ steps of an enumeration of the given [semidecidable axiomatization](../../../../../../semidecidable-axiomatization.md). These finite approximations can be computed in bounded time, even if the original axiom set is empty or finite. For each $\phi\in E_s$, form the precisely bracketed [logical conjunction](../../../../../../logical-conjunction.md)

$$
C_s(\phi)=\underbrace{(\cdots((\phi\wedge\phi)\wedge\phi)\cdots\wedge\phi)}_{s+1\text{ copies of }\phi},
$$

with $C_0(\phi)=\phi$. Let $D=\{C_s(\phi):\phi\in E_s,\ s\geq0\}$.

Each $C_s(\phi)$ is logically equivalent to $\phi$, so all members of $D$ follow from the original axioms. Every original axiom eventually belongs to some $E_s$, and its corresponding member $C_s(\phi)$ implies it. Hence $D$ axiomatizes exactly the same theory.

To decide whether a candidate sentence $\psi$ belongs to $D$, let $N$ be its syntactic length. A conjunction of $s+1$ copies has length at least $s+1$, so a representation $\psi=C_s(\phi)$ can only use $s<N$. Compute each $E_s$ for $s<N$, construct its finitely many candidates, and compare them literally with $\psi$. This finite procedure always terminates and accepts exactly $D$. It does not wait for a nonexistent next axiom, nor assume that conjunction parsing determines the original repeated formula uniquely. Thus **$D$ is a decidable equivalent axiomatization**, proving the [Craig trick](../../../../../../craig-trick.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
