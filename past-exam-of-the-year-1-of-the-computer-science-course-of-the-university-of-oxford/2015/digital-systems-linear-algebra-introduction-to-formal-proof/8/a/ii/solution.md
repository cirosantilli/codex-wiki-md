<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose an [eigenvariable](../../../../../../eigenvariable.md) $v$ fresh for the premise. Use the [existential quantifier introduction rule](../../../../../../existential-quantifier-introduction-rule.md) to contradict the premise under a [temporary assumption](../../../../../../temporary-assumption.md) $R(v)$:

$$
\begin{array}{rll}
1&\neg\exists x\,R(x)&\text{premise}\\
2&\vert\ R(v)&\text{assumption; }v\text{ fresh}\\
3&\vert\ \exists x\,R(x)&\exists\text{-intro }2\\
4&\vert\ \bot&\neg\text{-elim }3,1\\
5&\neg R(v)&\neg\text{-intro }2\text{--}4\\
6&\forall y\,\neg R(y)&\forall\text{-intro }5
\end{array}
$$

At line 6 the assumption $R(v)$ has been discharged and the sole remaining premise has no free $v$, satisfying the [eigenvariable condition](../../../../../../eigenvariable-condition.md). Thus

$$
\boxed{\neg\exists x\,R(x)\ \vdash\ \forall y\,\neg R(y).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
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
