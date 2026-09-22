<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [triangle embedding lemma for regular pairs](../../../../../../triangle-embedding-lemma-for-regular-pairs.md) states that if $0<\varepsilon<1/2$, the three pairs among disjoint nonempty sets $A,B,C$ are $\varepsilon$-uniform, and all three densities are at least $2\varepsilon$, then the graph contains a triangle with one vertex in each set.

In an $\varepsilon$-uniform pair $(A,B)$ of density $d$, fewer than $\varepsilon|A|$ vertices of $A$ have fewer than $(d-\varepsilon)|B|$ neighbours in $B$; otherwise those vertices and $B$ would violate uniformity. Apply this observation to $(A,B)$ and $(A,C)$. Since $2\varepsilon<1$, choose $a\in A$ that is typical for both pairs. Then

$$
B'=N(a)\cap B,qquad C'=N(a)\cap C
$$

satisfy $|B'|\geq\varepsilon|B|$ and $|C'|\geq\varepsilon|C|$. Uniformity of $(B,C)$ gives

$$
d(B',C')\geq d(B,C)-\varepsilon\geq\varepsilon>0.
$$

**Thus some $bc$ joins $B'$ to $C'$, and $abc$ is the required triangle.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
