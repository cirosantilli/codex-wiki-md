<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Measure the work of producing the entire output [list](../../../../../list-abstract-data-type.md), with constant-cost labels. Count height in levels, so a leaf has height one and $h=0$. A [perfect ternary tree](../../../../../perfect-ternary-tree.md) with $h+1$ levels has

$$
N_h=1+3+\cdots+3^h=\frac{3^{h+1}-1}{2}
$$

[vertices](../../../../../vertex-graph-theory.md). This is the [finite geometric series](../../../../../finite-geometric-series.md) formula, used without a new proof.

The three recursive calls cost $3T(h-1)$. Ordinary `concat = foldr (++) []` copies each immediate child result once, and each result has $N_{h-1}$ elements. Consequently the nonrecursive work is $\Theta(3N_{h-1}+1)=\Theta(3^h)$, giving

$$
T(0)=\Theta(1),\qquad T(h)=3T(h-1)+\Theta(3^h)\quad(h\geq1).
$$

Unroll this [recurrence relation](../../../../../recurrence-relation.md). At level $j$, the cost is $3^j\Theta(3^{h-j})=\Theta(3^h)$, and there are $h$ internal levels, followed by $3^h$ leaves. Therefore

$$
\boxed{T(\mathrm{flatten})(h)=\Theta((h+1)3^h)}.
$$

For $h\geq1$ this is conventionally written $\Theta(h3^h)$; in terms of total size it is $\Theta(N_h\log N_h)$. The extra height factor comes from copying labels at successive ancestors, even under [lazy evaluation](../../../../../lazy-evaluation.md) when the whole output is demanded. Merely producing its first constructor is a different cost question. If height instead counts edges, the source's height $h+1$ means $h+2$ levels; shifting the index by one leaves the boxed asymptotic bound unchanged. Part (c)'s suffix-passing implementation avoids this repeated copying.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
