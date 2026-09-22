<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [structural induction](../../../../../structural-induction.md) on the finite [list](../../../../../list-abstract-data-type.md) `xs`, strengthening the [induction hypothesis](../../../../../induction-hypothesis.md) to hold for every accumulator value $y$. For the empty [list](../../../../../list-abstract-data-type.md), the defining equation of the [left fold](../../../../../left-fold.md) gives

$$
x\oplus\operatorname{foldl}(\otimes)\,y\,[]
=x\oplus y
=\operatorname{foldl}(\otimes)\,(x\oplus y)\,[].
$$

For the inductive step, suppose the identity holds for the tail `zs` and every accumulator. Expand the first [left fold](../../../../../left-fold.md), apply the [induction hypothesis](../../../../../induction-hypothesis.md) at accumulator $y\otimes z$, and then use the supplied compatibility law:

$$
\begin{aligned}
x\oplus\operatorname{foldl}(\otimes)\,y\,(z:\mathrm{zs})
&=x\oplus\operatorname{foldl}(\otimes)\,(y\otimes z)\,\mathrm{zs}\\
&=\operatorname{foldl}(\otimes)\,(x\oplus(y\otimes z))\,\mathrm{zs}\\
&=\operatorname{foldl}(\otimes)\,((x\oplus y)\otimes z)\,\mathrm{zs}\\
&=\operatorname{foldl}(\otimes)\,(x\oplus y)\,(z:\mathrm{zs}).
\end{aligned}
$$

Hence

$$
\boxed{x\oplus\operatorname{foldl}(\otimes)\,y\,\mathrm{xs}=\operatorname{foldl}(\otimes)\,(x\oplus y)\,\mathrm{xs}.}
$$

Only equation (1) is needed for this part; the seed condition in equation (2) enters the next proof. Quantifying over the accumulator is essential because the recursive call changes it.

## ↑ Ancestors (12)

1. [A](../a.md)
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
