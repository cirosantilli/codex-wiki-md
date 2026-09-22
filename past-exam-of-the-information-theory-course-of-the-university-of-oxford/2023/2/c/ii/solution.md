<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For fixed $\varepsilon>0$, the [asymptotic equipartition property](../../../../../asymptotic-equipartition-property.md) gives $\Pr(X^n\notin A^{n,\varepsilon})\to0$. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) applied to $X_i$, which are bounded because their numerical [alphabet](../../../../../alphabet.md) is finite, gives $\Pr(X^n\notin B^{n,\varepsilon})\to0$. The [union bound](../../../../../boole-s-inequality.md) therefore yields

$$
\Pr(X^n\in S_n)\geq1-\Pr(X^n\notin A^{n,\varepsilon})-\Pr(X^n\notin B^{n,\varepsilon})\longrightarrow1.
$$

Since $\delta>0$, eventually $\Pr(X^n\in S_n)\geq2^{-\delta}$. Each word in $S_n$ has [probability mass](../../../../../probability-mass.md) at most $2^{-n(H(p)-\varepsilon)}$, so

$$
2^{-\delta}\leq\Pr(X^n\in S_n)
\leq |S_n|2^{-n(H(p)-\varepsilon)}.
$$

Rearranging proves

$$
\boxed{|A^{n,\varepsilon}\cap B^{n,\varepsilon}|\geq2^{n(H(p)-\varepsilon)-\delta}}
$$

for sufficiently large $n$. The key is that the factor $2^{-\delta}$ is a fixed number below one, however small $\delta$ is. This is an instance of [typical sets with an additional high-probability constraint](../../../../../typical-sets-with-an-additional-high-probability-constraint.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
