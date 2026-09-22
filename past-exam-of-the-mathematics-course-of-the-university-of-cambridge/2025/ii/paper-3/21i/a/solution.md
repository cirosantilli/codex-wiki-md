<h1 id="21i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) in sequential form states: if $K$ is a compact metric space and $(f_n)$ is a uniformly bounded, equicontinuous sequence in $C(K)$, then it has a uniformly convergent subsequence. Equivalently, a subset of $C(K)$ is relatively compact in the uniform norm exactly when it is uniformly bounded and equicontinuous.

For sufficiency, choose a finite $1/m$-net $E_m\subset K$ for every $m$. The union $D=\bigcup_mE_m$ is countable and dense. Uniform boundedness makes each scalar sequence $(f_n(x))_n$, $x\in D$, bounded. Successive applications of Bolzano-Weierstrass followed by a diagonal choice give a subsequence $(g_n)$ for which $g_n(x)$ converges at every $x\in D$.

Given $\varepsilon>0$, equicontinuity supplies $\delta>0$ such that

$$
d(x,y)<\delta\quad\Longrightarrow\quad
|g_n(x)-g_n(y)|<\varepsilon/3
$$

for every $n$. Choose a finite $\delta$-net from $D$. Pointwise convergence on those finitely many points makes $(g_n)$ uniformly Cauchy on the net, and the two equicontinuity estimates make it uniformly Cauchy on all of $K$. Since $C(K)$ is complete, $g_n$ converges uniformly.

Conversely, a relatively compact family is uniformly bounded because its closure is compact in the normed space $C(K)$. Given $\varepsilon>0$, cover that compact closure by finitely many uniform balls of radius $\varepsilon/3$, centred at continuous functions $h_1,\ldots,h_r$. Uniform continuity of the finitely many $h_i$ gives one $\delta$ that works for all of them. Approximating any family member by one $h_i$ proves equicontinuity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21I](../../21i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
