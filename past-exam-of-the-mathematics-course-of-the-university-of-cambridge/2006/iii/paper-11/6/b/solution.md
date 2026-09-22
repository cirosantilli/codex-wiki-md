<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
h(M)=x^*_{M\setminus\{\min M\}}(x_{\min M}).
$$

This scalar function is continuous. The first element is locally constant; deleting it is continuous on increasing sequences; and evaluation on a fixed $x_m$ is continuous in the [weak-star topology](../../../../../../weak-star-topology.md). Thus $\mathcal U=\{M:|h(M)|<\delta\}$ is open.

By part (a), choose an infinite $L_0$ homogeneous for $\mathcal U$. If all its infinite subsets are in $\mathcal U$, the required conclusion follows. Suppose instead every one has $|h(M)|\geq\delta$. Choose finitely many unit scalars $\zeta_1,\ldots,\zeta_q$ such that every scalar $z$ with $|z|\geq\delta$ has $\operatorname{Re}(\zeta_jz)>\delta/2$ for some $j$; for real scalars the two signs suffice. The open sets

$$
\mathcal U_j=\{M:\operatorname{Re}(\zeta_jh(M))>\delta/2\}
$$

cover $[L_0]^\omega$. Apply the open [Ramsey set of infinite subsets](../../../../../../ramsey-set-of-infinite-subsets.md) result successively to them. After finitely many refinements, at least one, say $\mathcal U_j$, contains every infinite subset of a remaining infinite $L$; otherwise their cover would be violated.

For any finite $F\subseteq L$, choose an infinite $N\subseteq L$ after $\max F$. For each $m\in F$, apply this homogeneity to $M=\{m\}\cup N$. Its deleted tail is always the same $N$, so the same functional satisfies

$$
\operatorname{Re}(\zeta_jx_N^*(x_m))>\delta/2\qquad(m\in F).
$$

But $(x_m)_{m\in L}$ is a [weakly null sequence](../../../../../../weakly-null-sequence.md). The [Mazur lemma](../../../../../../mazur-s-lemma.md) gives a finite convex combination $z=\sum_{m\in F}\lambda_mx_m$ with $\|z\|<\delta/2$. The displayed inequalities give $\operatorname{Re}(\zeta_jx_N^*(z))>\delta/2$, contradicting $\|x_N^*\|\leq1$. The bad homogeneous case is impossible. Therefore

$$
\boxed{|x^*_{M'}(x_m)|<\delta\quad\text{for every }M\in[L]^\omega,\quad m=\min M,\ M'=M\setminus\{m\}.}
$$

Continuity is used to make the scalar tests open; weak nullity is used only for the finite convex-combination contradiction. The argument works over both real and complex scalars.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
