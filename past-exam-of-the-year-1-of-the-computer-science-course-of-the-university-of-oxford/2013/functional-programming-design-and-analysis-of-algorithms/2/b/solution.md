<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Again use [structural induction](../../../../../structural-induction.md) on the finite [list](../../../../../list-abstract-data-type.md). At `[]`, both the [right fold](../../../../../list-fold.md) and the [left fold](../../../../../left-fold.md) return the seed $a$. If they agree on `zs`, then

$$
\begin{aligned}
\operatorname{foldr}(\oplus)\,a\,(z:\mathrm{zs})
&=z\oplus\operatorname{foldr}(\oplus)\,a\,\mathrm{zs}\\
&=z\oplus\operatorname{foldl}(\otimes)\,a\,\mathrm{zs}\\
&=\operatorname{foldl}(\otimes)\,(z\oplus a)\,\mathrm{zs}\\
&=\operatorname{foldl}(\otimes)\,(a\otimes z)\,\mathrm{zs}\\
&=\operatorname{foldl}(\otimes)\,a\,(z:\mathrm{zs}).
\end{aligned}
$$

The third line uses part (a); the fourth uses equation (2). Thus the [left-right fold equivalence](../../../../../left-right-fold-equivalence.md) is

$$
\boxed{\operatorname{foldr}(\oplus)\,a\,\mathrm{xs}=\operatorname{foldl}(\otimes)\,a\,\mathrm{xs}.}
$$

This is a statement about values on finite, total inputs. It does not assert equal evaluation costs or equal behaviour on infinite [lists](../../../../../list-abstract-data-type.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
