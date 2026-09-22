# Strong induction with four starting cases

↑ **Parent:** [Strong induction](strong-induction.md)

Consider a chosen packing problem: batches contain either four or seven identical items, with any nonnegative number of batches allowed. Which integer totals can be formed? The claim is that **every total of at least eighteen is attainable**:

$$
\forall n\geq18,\quad\exists a,b\in\mathbb N:\quad n=4a+7b.
$$

Here $a,b$ count batches, so they must be [nonnegative integers](natural-number.md); the convention $\mathbb N=\{0,1,2,\ldots\}$ permits omitting either size. Four direct starting cases are

$$
18=4+7+7,\qquad19=4+4+4+7,\qquad20=4+4+4+4+4,\qquad21=7+7+7.
$$

If $n\geq21$ and every total from $18$ through $n$ is attainable, then $n-3\geq18$ is one of the cases available in the [induction hypothesis](induction-hypothesis.md). Add a batch of four to its representation to obtain $n+1$. Thus the [inductive step](inductive-step.md) applies to every new total from $22$ onward. Formally, one can start the [strong induction](strong-induction.md) at $18$ and handle the next three totals directly before using the uniform step. The finite checks and the propagation together establish all totals, not merely those drawn below.

<a id="image-four-starting-cases-seed-every-residue-class-when-the-step-adds-four"></a>
![](strong-induction-four-seven-starting-cases.png)

**[Figure 4](#image-four-starting-cases-seed-every-residue-class-when-the-step-adds-four). Four starting cases seed every residue class when the step adds four**. Original chosen batch sizes $4$ and $7$. Colored rows follow $18,22,26,\ldots$; $19,23,27,\ldots$; $20,24,28,\ldots$; and $21,25,29,\ldots$. Each arrow adds a batch of four. The lower strip exhaustively checks totals through $29$; a cross means no representation by nonnegative batch counts. The infinite conclusion comes from the [inductive step](inductive-step.md), not from this finite enumeration.

Checking only $18$ and repeatedly adding four would reach only totals congruent to $18$ in [modular arithmetic](modular-arithmetic-split.md) modulo four. The four [induction base cases](induction-base-case.md) supply all four [residue classes](residue-class.md). The number of starting cases comes from this chosen construction, not from a universal requirement that [strong induction](strong-induction.md) needs several bases. A different construction can need different starting information.

The threshold is sharp for these batch sizes. If $17=4a+7b$, reducing modulo four gives $3b\equiv1\pmod4$, so $b\equiv3\pmod4$. A nonnegative $b$ would therefore be at least three, giving $7b\geq21>17$, a [contradiction](contradiction.md). A finite failed search alone would need an explicit bound on $a,b$; this short [modular arithmetic](modular-arithmetic-split.md) argument supplies a general obstruction.

## ↑ Ancestors (7)

1. [Strong induction](strong-induction.md)
2. [Mathematical induction](mathematical-induction.md)
3. [Mathematical proof](mathematical-proof.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
