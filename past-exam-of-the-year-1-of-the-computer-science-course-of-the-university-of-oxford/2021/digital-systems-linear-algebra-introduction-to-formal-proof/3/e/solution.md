<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The five maximal four-cell groups give the [disjunctive normal form](../../../../../disjunctive-normal-form.md)

$$
\boxed{z=a_1\neg b_1\lor a_1a_0\lor a_1\neg b_0\lor a_0\neg b_1\lor\neg b_1\neg b_0.}
$$

For example, the group $a_1\neg b_0$ wraps between columns $00$ and $10$ in the bottom two rows. No group of eight cells is entirely one. The five terms are precisely the [prime implicants](../../../../../prime-implicant.md), and each is essential: respectively, the cells $(a,b)=(2,1),(3,3),(2,2),(1,1),(0,0)$ are covered by no other [prime implicant](../../../../../prime-implicant.md). Any [disjunctive normal form](../../../../../disjunctive-normal-form.md) can have its terms enlarged to [prime implicants](../../../../../prime-implicant.md) without increasing its size. Therefore all five displayed terms are necessary, proving minimality in number of products; each needs two [literals](../../../../../boolean-literal.md), also giving ten [literals](../../../../../boolean-literal.md) in a minimal cover.

For an implementation with [AND gates](../../../../../and-gate.md) and [NOT gates](../../../../../not-gate.md), call these five products $T_1,\ldots,T_5$. Form the shared complements $\neg b_1,\neg b_0$, calculate each $T_i$ with an [AND gate](../../../../../and-gate.md), invert every $T_i$, and use

$$
z=\neg\bigl(\neg T_1\land\neg T_2\land\neg T_3\land\neg T_4\land\neg T_5\bigr).
$$

A five-input conjunction can be replaced by four two-input [AND gates](../../../../../and-gate.md). This direct implementation uses nine two-input [AND gates](../../../../../and-gate.md) and eight [NOT gates](../../../../../not-gate.md). That is a valid realization of the minimal [disjunctive normal form](../../../../../disjunctive-normal-form.md), rather than a claim that this particular gate count is globally optimal among all factored circuits.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
