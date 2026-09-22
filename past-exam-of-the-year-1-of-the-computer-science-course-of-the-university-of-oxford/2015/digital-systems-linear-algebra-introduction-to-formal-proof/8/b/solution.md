<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a fresh [existential witness](../../../../../existential-witness.md) $v$. Within the assumption of the forbidden [universal quantification](../../../../../universal-quantification.md), eliminate the original [existential quantification](../../../../../existential-quantification.md) to obtain [logical falsity](../../../../../logical-falsity.md):

$$
\begin{array}{rll}
1&\exists x\,R(x)&\text{premise}\\
2&\vert\ \forall y\,\neg R(y)&\text{assumption}\\
3&\vert\ \vert\ R(v)&\text{witness assumption; }v\text{ fresh}\\
4&\vert\ \vert\ \neg R(v)&\forall\text{-elim }2\\
5&\vert\ \vert\ \bot&\neg\text{-elim }3,4\\
6&\vert\ \bot&\exists\text{-elim }1,3\text{--}5\\
7&\neg\forall y\,\neg R(y)&\neg\text{-intro }2\text{--}6
\end{array}
$$

The witness $v$ appears neither in the exported conclusion $\bot$ at line 6 nor in the other undischarged assumptions. The [existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md) is therefore valid, and

$$
\boxed{\exists x\,R(x)\ \vdash\ \neg\forall y\,\neg R(y).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
