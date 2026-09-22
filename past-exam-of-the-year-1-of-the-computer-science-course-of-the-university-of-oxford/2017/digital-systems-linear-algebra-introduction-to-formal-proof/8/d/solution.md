<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $H=\exists y\,\forall x\,R(x,y)$. For the first proof, eliminate the common witness before introducing the universal quantifier. Choose fresh $b$ and a further fresh arbitrary $a$:

$$
\begin{array}{rll}
1&H&\text{premise}\\
2&\quad\forall x\,R(x,b)&\text{fresh witness assumption}\\
3&\quad R(a,b)&\forall E\ 2\\
4&\quad\exists y\,R(a,y)&\exists I\ 3\\
5&\quad\forall x\,\exists y\,R(x,y)&\forall I\ 4\\
6&\forall x\,\exists y\,R(x,y)&\exists E\ 1,2\text{--}5
\end{array}
$$

At line 5, $a$ occurs free in neither $H$ nor the witness assumption, so [universal introduction](../../../../../universal-quantifier-introduction-rule.md) is valid. At line 6, $b$ is absent from the conclusion and other open assumptions.

For the second proof, reserve arbitrary $a$, eliminate the common witness only as far as the particular existential, close that subproof, and then generalize:

$$
\begin{array}{rll}
1&H&\text{premise}\\
2&\quad\forall x\,R(x,b)&\text{fresh witness assumption}\\
3&\quad R(a,b)&\forall E\ 2\\
4&\quad\exists y\,R(a,y)&\exists I\ 3\\
5&\exists y\,R(a,y)&\exists E\ 1,2\text{--}4\\
6&\forall x\,\exists y\,R(x,y)&\forall I\ 5
\end{array}
$$

At line 5 the exported formula contains no free $b$; at line 6 the only open assumption $H$ contains no free $a$. These different orders of [assumption discharge](../../../../../assumption-discharge.md) both respect the [eigenvariable condition](../../../../../eigenvariable-condition.md).

**The converse is not valid.** On the domain $\{0,1\}$, interpret $R(x,y)$ as $x=y$. Each $x$ has a witness $y=x$, so $\forall x\,\exists y\,R(x,y)$ holds, but no single $y$ equals both elements. Thus $\exists y\,\forall x\,R(x,y)$ is false. This is precisely the distinction in [quantifier order and uniform witness](../../../../../quantifier-order-and-uniform-witness.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
