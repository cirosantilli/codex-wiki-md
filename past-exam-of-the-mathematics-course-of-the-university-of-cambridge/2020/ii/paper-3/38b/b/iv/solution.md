<h1 id="38b/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Set

$$
F(\eta)=f'(\eta)
=\frac{5-\cosh z}{1+\cosh z},
\qquad
z=\sqrt2\eta+c.
$$

Writing $C=\cosh z$, direct differentiation gives

$$
F''(\eta)=\frac{12(C-2)}{(1+C)^2}.
$$

On the other hand,

$$
1-F^2
=\frac{(1+C)^2-(5-C)^2}{(1+C)^2}
=\frac{12(C-2)}{(1+C)^2}.
$$

Thus $F''=1-F^2$, which is precisely $f'''=1-(f')^2$. The far-field condition is automatic because $F\to-1$. No slip requires

$$
0=F(0)=\frac{5-\cosh c}{1+\cosh c},
$$

so

$$
\boxed{c=\pm\operatorname{arcosh}5}.
$$

For $c=+\operatorname{arcosh}5$, $F$ decreases directly from $0$ to $-1$, matching flow everywhere toward the sink. For the negative root, $F$ initially becomes positive and creates a reverse-flow region next to the wall. The physically likely choice is therefore

$$
\boxed{c=+\operatorname{arcosh}5}.
$$

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [38B](../../../38b.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
