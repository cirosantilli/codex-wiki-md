<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $S_n=n^{-1/2}\sum_{k=1}^nX_k$. By [independence of random variables](../../../../../independent-random-variables.md), its [moment-generating function](../../../../../moment-generating-function.md) is

$$
M_{S_n}(t)=M_X(t/\sqrt n)^n.
$$

For each fixed real $t$, the expansion in part (i) yields

$$
\log M_{S_n}(t)
=n\left(\frac{t^2}{2n}+o(n^{-1})\right)
\longrightarrow\frac{t^2}{2}.
$$

For $t=0$ the equality is immediate. Exponentiation gives $M_{S_n}(t)\to e^{t^2/2}$, the [moment-generating function of a standard normal variable](../../../../../moment-generating-function-of-a-standard-normal-variable.md). The functions are finite on a common neighborhood of zero, so the [convergence theorem for moment-generating functions](../../../../../convergence-theorem-for-moment-generating-functions.md) proves

$$
\boxed{S_n\xrightarrow dN(0,1).}
$$

This proves the [central limit theorem](../../../../../central-limit-theorem.md) under the exponential-moment hypothesis of this part.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
