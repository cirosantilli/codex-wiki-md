<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First suppose $m(E)<\infty$. The interval-cover definition of [Lebesgue outer measure](../../../../../lebesgue-outer-measure.md), together with $m^*(E)=m(E)$, provides bounded open intervals $I_j$ covering $E$ such that $\sum_j|I_j|<m(E)+\varepsilon$. If the definition uses intervals that are not open, enlarge each by an amount whose total is smaller than the available error. For the [open set](../../../../../open-set.md) $U=\bigcup_j I_j$, [countable subadditivity](../../../../../countable-subadditivity-of-a-measure.md) and additivity of [Lebesgue measure](../../../../../lebesgue-measure.md) give

$$
m(U\setminus E)=m(U)-m(E)\leq\sum_j|I_j|-m(E)<\varepsilon.
$$

This subtraction is valid because both measures are finite.

For arbitrary $E$, including $m(E)=\infty$, set $E_n=E\cap[n,n+1)$ for $n\in\mathbb Z$, and choose positive weights $w_n=2^{-|n|}/3$, whose sum is one. Each $E_n$ has finite [Lebesgue measure](../../../../../lebesgue-measure.md), so the preceding argument gives an [open set](../../../../../open-set.md) $U_n\supseteq E_n$ with $m(U_n\setminus E_n)<\varepsilon w_n$. Then $U=\bigcup_{n\in\mathbb Z}U_n$ is open, contains $E$, and

$$
\boxed{m(U\setminus E)\leq\sum_{n\in\mathbb Z}m(U_n\setminus E_n)<\varepsilon.}
$$

Thus the required form of [regularity of Lebesgue measure](../../../../../regularity-of-lebesgue-measure.md) does not require $E$ itself to have finite measure.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
