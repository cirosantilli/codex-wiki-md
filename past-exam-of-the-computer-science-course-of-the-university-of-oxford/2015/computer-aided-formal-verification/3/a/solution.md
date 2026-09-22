<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $A=\operatorname{Sat}(\Phi)\subseteq S$. All arguments depend only on this given [satisfaction set](../../../../../satisfaction-set.md); they do not require an additional convention for the printed notation $\Phi\in2^{AP}$. For a [state](../../../../../state-computer-science.md) $s$, let $\operatorname{Post}(s)=\{t:s\to t\}$. The [power set](../../../../../power-set.md) $2^S$ is ordered by [set inclusion](../../../../../set-inclusion.md).

Take $X\subseteq Y\subseteq S$ and any $s\in H(X)$. By the definition of $H$, we have both $s\in A$ and $\operatorname{Post}(s)\subseteq X$. By transitivity of [set inclusion](../../../../../set-inclusion.md), $\operatorname{Post}(s)\subseteq Y$, so $s\in H(Y)$. Since this applies to every member of $H(X)$,

$$
\boxed{X\subseteq Y\ \Longrightarrow\ H(X)\subseteq H(Y).}
$$

Thus $H$ is an [order-preserving function](../../../../../order-preserving-function.md), which is the meaning of monotonicity here. This proof does not need either finiteness or the absence of [terminal states](../../../../../terminal-state.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
