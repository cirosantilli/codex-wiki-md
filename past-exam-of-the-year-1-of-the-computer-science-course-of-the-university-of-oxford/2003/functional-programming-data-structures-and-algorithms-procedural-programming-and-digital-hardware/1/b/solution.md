<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [structural induction](../../../../../structural-induction.md) on the first finite outer [list](../../../../../list-abstract-data-type.md) `xss`, with the assertion quantified over every finite `yss`. For `xss = []`, both sides are `[]`. For the nonempty case of [structural induction](../../../../../structural-induction.md), write `xss = xs:xss'`. If `yss = []`, both sides again truncate to `[]`. Otherwise write `yss = ys:yss'`. Expanding the definitions gives

$$
\begin{aligned}
&\operatorname{combine}(\operatorname{map}(z:)(xs:xss'))(ys:yss')\\
&\quad=((z:xs)\mathbin{++}ys):\operatorname{combine}(\operatorname{map}(z:)xss')yss'\\
&\quad=(z:(xs\mathbin{++}ys)):\operatorname{map}(z:)(\operatorname{combine}xss'\,yss')\\
&\quad=\operatorname{map}(z:)\big((xs\mathbin{++}ys):\operatorname{combine}xss'\,yss'\big)\\
&\quad=\operatorname{map}(z:)(\operatorname{combine}(xs:xss')(ys:yss')).
\end{aligned}
$$

The second equality uses the defining equation for [list concatenation](../../../../../list-concatenation.md) and the [induction hypothesis](../../../../../induction-hypothesis.md) for the smaller outer [list](../../../../../list-abstract-data-type.md) `xss'`. The argument covers unequal outer lengths because the empty second [list](../../../../../list-abstract-data-type.md) was handled explicitly. Hence

$$
\boxed{\operatorname{combine}(\operatorname{map}(z:)xss)yss
=\operatorname{map}(z:)(\operatorname{combine}xss\,yss).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
