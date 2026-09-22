<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use three [D flip-flops](../../../../../d-flip-flop.md) whose stored [bits](../../../../../bit.md) $A,B,C$ represent $4A+2B+C$. Initialize them to $000$. The [Moore machine](../../../../../moore-machine.md)'s output is this stored [binary representation](../../../../../binary-number.md), and its [state transition table](../../../../../state-transition-table.md) is:

| Present $ABC$ | Next $A^+B^+C^+$ |
| --- | --- |
| $000$ | $001$ |
| $001$ | $010$ |
| $010$ | $011$ |
| $011$ | $100$ |
| $100$ | $101$ |
| $101$ | $000$ |

Treat the two unused [state encodings](../../../../../state-encoding.md) $110,111$ as [don't-care conditions](../../../../../don-t-care-term.md) when minimizing the [sum of products](../../../../../disjunctive-normal-form.md). With juxtaposition for AND, $+$ for OR and a bar for NOT, one minimal choice is

$$
\boxed{D_A=A\overline C+BC,\qquad D_B=B\overline C+\overline A\,\overline B C,\qquad D_C=\overline C.}
$$

For $D_A$, the required ones at $011$ and $100$ cannot share one valid [implicant](../../../../../implicant.md): their differing [bits](../../../../../bit.md) would force inclusion of required zeros. Pair $011$ with the unused $111$ to get $BC$, and $100$ with unused $110$ to get $A\overline C$. Neither term can lose a [Boolean literal](../../../../../boolean-literal.md) without covering a required zero.

For $D_B$, state $001$ is isolated from every other required one and from the unused states by required zeros, so it forces the three-[Boolean literal](../../../../../boolean-literal.md) term $\overline A\,\overline B C$. State $010$ pairs with unused $110$ to give $B\overline C$. Finally $D_C=\overline C$ is a single [Boolean literal](../../../../../boolean-literal.md). Thus the three expressions are minimal [sum of products](../../../../../disjunctive-normal-form.md) expressions under the stated unused-state convention. In fact these choices also recover from $110\to111\to100$, so initialization into an unused state eventually joins the intended [modulo-six counter](../../../../../modulo-six-counter.md) cycle.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
