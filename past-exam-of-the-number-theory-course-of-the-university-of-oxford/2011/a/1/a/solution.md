<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [splitting field](../../../../../splitting-field.md) of a nonconstant [polynomial](../../../../../polynomial-split.md) $f$ over a [field](../../../../../field.md) $K$ is an [field extension](../../../../../field-extension.md) $L$ in which $f$ factors into linear factors and which is generated over $K$ by those roots. We prove existence and the divisibility simultaneously by induction on $n=\deg f$; constant nonzero polynomials have [splitting field](../../../../../splitting-field.md) $K$.

If $f$ is reducible, write $f=gh$ with positive degrees $r,s<n$. By induction first split $g$, obtaining $E/K$ of degree dividing $r!$, then split $h$ over $E$, obtaining $L/E$ of degree dividing $s!$. The [tower law for field extensions](../../../../../tower-law-for-field-extensions.md) gives $[L:K]\mid r!s!\mid(r+s)!$. All adjoined elements are roots of $f$, so $L$ has the required minimality.

If $f$ is irreducible, take $E=K[x]/(f)$ and let $\alpha$ be the image of $x$. Then $[E:K]=n$ and $f=(x-\alpha)h$ in $E[x]$. Apply induction to $h$, of degree $n-1$, to obtain $[L:E]\mid(n-1)!$. Therefore

$$
\boxed{[L:K]=n[L:E]\mid n!.}
$$

This proof also covers inseparable polynomials; it does not incorrectly identify extension degree with [automorphism](../../../../../automorphism.md) count in that case.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the number theory course of the University of Oxford](../../../../split.md)
6. [Number theory course of the University of Oxford](../../../../../number-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
