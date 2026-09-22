<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Freiman-Ruzsa theorem over a finite field](../../../../../../freiman-ruzsa-theorem-over-a-finite-field.md) states that if $A\subseteq\mathbb F_p^n$ and $|A+A|\leq K|A|$, then $A$ is contained in a [vector subspace](../../../../../../vector-subspace.md) $H$ with

$$
|H|\leq K^2p^{K^4}|A|.
$$

After translating $A$, assume $0\in A$. Put $S=A-A$, and choose $X\subseteq A+S$ maximal subject to the translates $x+A$, $x\in X$, being pairwise disjoint. Since $X+A\subseteq2A+S=3A-A$, the [Plünnecke-Ruzsa inequality](../../../../../../plunnecke-ruzsa-inequality.md) gives

$$
|X||A|=|X+A|\leq|3A-A|\leq K^4|A|,
$$

so $|X|\leq K^4$.

Maximality gives $A+S\subseteq X+S$: if $y\in A+S$ is not already in $X$, then $(y+A)\cap(x+A)\ne\varnothing$ for some $x\in X$, whence $y\in x+A-A=x+S$. Inductively, $mA+S\subseteq\langle X\rangle+S$ for every positive integer $m$. Because $0\in A$, every element of $\langle A\rangle$ belongs to some $mA$ in the finite vector space, and therefore

$$
H:=\langle A\rangle\subseteq\langle X\rangle+S.
$$

Finally, $|\langle X\rangle|\leq p^{|X|}$ and $|S|\leq K^2|A|$ by the Plünnecke-Ruzsa inequality, so

$$
\boxed{|H|\leq p^{|X|}|S|\leq K^2p^{K^4}|A|.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
