<h1 id="4f/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [regular concatenation grammar](../../../../../../../regular-concatenation-grammar.md), let

$$
P_1=
\{\alpha\to\beta\in P:\beta\notin\Sigma^*\}
\cup
\{\alpha\to wS':(\alpha\to w)\in P,\ w\in\Sigma^*\}.
$$

Then define

$$
H^{\mathrm{reg}}=(\Sigma,V\cup V',P_1\cup P',S).
$$

If $G$ and $G'$ are regular, every nonterminal rule retained from $P$ is right-linear, and each replaced terminal rule is also right-linear. A regular derivation in $G$ uses exactly one terminal rule, at its final step; the replacement transfers control to $S'$, after which a word of $L(G')$ is generated. Hence

$$
\boxed{L(H^{\mathrm{reg}})=L(G)L(G').}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4F](../../../4f.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
