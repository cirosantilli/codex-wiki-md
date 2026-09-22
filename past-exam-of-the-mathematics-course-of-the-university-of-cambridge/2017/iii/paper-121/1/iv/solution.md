<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

First prove [set-theoretic absoluteness](../../../../../../set-theoretic-absoluteness.md) for syntactically [bounded formulas in set theory](../../../../../../bounded-formula-in-set-theory.md) by induction on their construction. Atomic equality and membership use the actual equality and membership relations in both [transitive classes](../../../../../../transitive-class.md). [Boolean operations](../../../../../../boolean-operation.md) preserve agreement.

For the bounded existential step, take $a\in M$ and suppose $N\models\exists u\in a\,\psi(u,\vec b)$. Its witness $c$ is an actual member of $a$. Since $M$ is a [transitive class](../../../../../../transitive-class.md), $c\in M$; the induction hypothesis then gives $M\models\psi(c,\vec b)$. The converse uses the same witness in $N$. The bounded universal step follows similarly because both structures quantify over exactly the actual members of $a$, or follows by [negation](../../../../../../negation.md) from the existential step. Hence

$$
\boxed{\psi^M(\vec b)\leftrightarrow\psi^N(\vec b)\qquad\text{for every syntactic }\Delta_0\text{ formula and }\vec b\in M.}
$$

No [ZF](../../../../../../zermelo-fraenkel-set-theory.md) axioms are needed for this syntactic statement beyond the ambient meaning of a [transitive class](../../../../../../transitive-class.md). For a [ZF-equivalent bounded formula](../../../../../../zf-equivalent-bounded-formula.md) $\varphi$, choose a bounded equivalent $\psi$. The assumption that both structures model [ZF](../../../../../../zermelo-fraenkel-set-theory.md) gives $\varphi^M\leftrightarrow\psi^M$ and $\varphi^N\leftrightarrow\psi^N$. Combining these with the displayed equivalence proves the asserted [set-theoretic absoluteness](../../../../../../set-theoretic-absoluteness.md) of $\Delta_0^{\mathrm{ZF}}$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
