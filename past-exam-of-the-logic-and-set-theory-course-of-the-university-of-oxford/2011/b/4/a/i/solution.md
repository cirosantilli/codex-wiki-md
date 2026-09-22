<h1 id="b/4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An approximation is a function $s:n+1\to X$ with $s(0)=x_0$ and $s(k+1)=g(s(k))$ for $k<n$. By induction on $n$, there is such a function: start with $\{(0,x_0)\}$ and append the uniquely specified value $g(s(n))$.

Any two approximations agree on their common domain, by induction from their common initial value and the same transition [function](../../../../../../function-split.md) $g$. The collection $\mathcal S$ of all approximations is a set, being a definable subset of $\mathcal P(\omega\times X)$. Therefore $f=\bigcup\mathcal S$ is a [function](../../../../../../function-split.md). Existence of approximations of every finite length gives $\operatorname{dom}(f)=\omega$. Each defining equation appears in a sufficiently long approximation, so

$$
\boxed{f:\omega\to X,\qquad f(0)=x_0,\qquad f(n+1)=g(f(n)).}
$$

This proves the [natural-number recursion theorem](../../../../../../natural-number-recursion-theorem.md) without the [axiom of choice](../../../../../../axiom-of-choice.md); no arbitrary sequence of choices was made.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [B](../../../../b.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
