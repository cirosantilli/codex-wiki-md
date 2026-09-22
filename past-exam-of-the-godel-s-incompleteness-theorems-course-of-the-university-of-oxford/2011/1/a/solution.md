<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $BA=P(\ulcorner A\urcorner)$, with the corner notation understood as the numeral for the [Gödel number](../../../../godel-number.md). An [arithmetical provability predicate](../../../../arithmetical-provability-predicate.md) numerates the theorems of $S$ in the standard natural numbers and satisfies the [Hilbert-Bernays-Löb derivability conditions](../../../../hilbert-bernays-lob-derivability-conditions.md):

$$
\begin{aligned}
& S\vdash A\quad\Longrightarrow\quad S\vdash BA,\qquad\text{an external rule;}\\
& S\vdash B(A\to C)\to(BA\to BC);\\
& S\vdash BA\to B(BA).
\end{aligned}
$$

The last two conditions are internal theorems, not rules authorizing reflection from $BA$ to $A$.

Here $P(x)=\exists y\,\operatorname{Prov}(x,y)$ numerates the theorem set by the given assumption. If $S\vdash A$, its proof supplies a genuine natural-number witness, making $BA$ a true [Sigma-1 formula](../../../../sigma-1-formula.md). [Sigma-1 completeness](../../../../sigma-1-completeness.md) gives $S\vdash BA$, proving the first condition. The second condition is supplied explicitly. Since $BA$ is itself a [Sigma-1 formula](../../../../sigma-1-formula.md), the given formalized [Sigma-1 completeness](../../../../sigma-1-completeness.md) yields $S\vdash BA\to B(BA)$, the third condition. Thus **the specified existential proof predicate is an [arithmetical provability predicate](../../../../arithmetical-provability-predicate.md)**.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
