<h1 id="7/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use [proof by contradiction](../../../../../../reductio-ad-absurdum.md), expanding the final classical step explicitly into [negation introduction](../../../../../../negation-introduction-rule.md) followed by [double-negation elimination](../../../../../../double-negation-elimination.md). First the assumption $\neg(\neg P\lor\neg Q)$ forces $P$: otherwise $\neg P$ immediately gives the prohibited [logical disjunction](../../../../../../logical-disjunction.md). It similarly forces $Q$. The formal [natural deduction](../../../../../../natural-deduction.md) derivation is

$$
\begin{array}{rll}
1&\neg(P\land Q)&\text{premise}\\
2&\vert\ \neg(\neg P\lor\neg Q)&\text{assumption}\\
3&\vert\ \vert\ \neg P&\text{assumption}\\
4&\vert\ \vert\ \neg P\lor\neg Q&\lor\text{-intro-L }3\\
5&\vert\ \vert\ \bot&\neg\text{-elim }4,2\\
6&\vert\ \neg\neg P&\neg\text{-intro }3\text{--}5\\
7&\vert\ P&\neg\neg\text{-elim }6\\
8&\vert\ \vert\ \neg Q&\text{assumption}\\
9&\vert\ \vert\ \neg P\lor\neg Q&\lor\text{-intro-R }8\\
10&\vert\ \vert\ \bot&\neg\text{-elim }9,2\\
11&\vert\ \neg\neg Q&\neg\text{-intro }8\text{--}10\\
12&\vert\ Q&\neg\neg\text{-elim }11\\
13&\vert\ P\land Q&\land\text{-intro }7,12\\
14&\vert\ \bot&\neg\text{-elim }13,1\\
15&\neg\neg(\neg P\lor\neg Q)&\neg\text{-intro }2\text{--}14\\
16&\neg P\lor\neg Q&\neg\neg\text{-elim }15
\end{array}
$$

Hence

$$
\boxed{\neg(P\land Q)\ \vdash\ \neg P\lor\neg Q.}
$$

This direction of [De Morgan's laws](../../../../../../de-morgan-s-laws.md) uses the classical rule supplied on the source rule sheet; it has not been silently treated as an available [inference rule](../../../../../../inference-rule.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
