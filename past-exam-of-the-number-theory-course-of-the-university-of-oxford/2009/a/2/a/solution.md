<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [splitting field](../../../../../splitting-field.md) is an extension in which the [polynomial](../../../../../polynomial-split.md) factors into linear factors and which is generated over the base [field](../../../../../field.md) by its roots. Prove existence together with the factorial divisibility by strong induction on $d$, with degrees zero and one immediate for a nonzero [polynomial](../../../../../polynomial-split.md).

If $f$ is reducible, write $f=gh$ with $1\le e=\deg g<d$, $\deg h=d-e$. By induction first split $g$ in $K_1/K$ with degree dividing $e!$, then split $h$ over $K_1$ with degree dividing $(d-e)!$. The resulting [field](../../../../../field.md) is generated over $K$ by all roots of $f$, hence is a [splitting field](../../../../../splitting-field.md). Its degree divides $e!(d-e)!$, which divides $d!$ because the binomial coefficient $d!/[e!(d-e)!]$ is an [integer](../../../../../integer-split.md).

If $f$ is irreducible, adjoin a root $\alpha$, obtaining degree $[K(\alpha):K]=d$. Over this [field](../../../../../field.md) divide out $X-\alpha$ and split the degree-$(d-1)$ quotient by induction. That [splitting field](../../../../../splitting-field.md) together with the base already contains every root and has degree over $K$ dividing $d(d-1)!=d!$. Thus

$$
\boxed{[L:K]\mid d!.}
$$

The reducible/irreducible distinction proves divisibility, not just an upper bound on the degree, and works without assuming separability.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the number theory course of the University of Oxford](../../../../split.md)
6. [Number theory course of the University of Oxford](../../../../../number-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
