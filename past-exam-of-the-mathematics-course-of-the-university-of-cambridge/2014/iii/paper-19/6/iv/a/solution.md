<h1 id="6/iv/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We construct a stronger family: every [injection](../../../../../../../injective-function.md) $e_\alpha:\alpha\to\omega$ will have coinfinite range, and coherence means agreement modulo finitely many arguments. Begin with the empty [function](../../../../../../../function-split.md). At a successor, extend $e_\alpha$ by assigning the new argument a value outside its range; the range remains coinfinite, and coherence with earlier [functions](../../../../../../../function-split.md) is unchanged.

At a countable limit $\alpha$, take $0=\alpha_0<\alpha_1<\cdots$ cofinal in $\alpha$. We build [injections](../../../../../../../injective-function.md) $p_n:\alpha_n\to\omega$, extending one another exactly, with $p_n$ differing from $e_{\alpha_n}$ at finitely many arguments. Also reserve distinct numbers $k_0,k_1,\ldots$, never used by the eventual union. After constructing $p_n$, choose $k_n$ outside its range and different from the earlier reserved numbers; its range is coinfinite since it differs finitely from that of $e_{\alpha_n}$.

To extend to $\alpha_{n+1}$, first use $e_{\alpha_{n+1}}$ on the new arguments while keeping $p_n$ on the old ones. Only finitely many collisions can arise: $p_n$ and $e_{\alpha_{n+1}}\upharpoonright\alpha_n$ differ finitely by the inductive coherence hypothesis, so their image [sets](../../../../../../../set-split.md) differ finitely. The candidate is otherwise injective. There are also only finitely many new arguments assigned a value among $k_0,\ldots,k_n$. Reassign these finitely many bad arguments to distinct fresh values outside the candidate image and the reserved [finite set](../../../../../../../finite-set.md). Infinitely many fresh values are available because the candidate image differs only finitely from the coinfinite image of $e_{\alpha_{n+1}}$. The resulting $p_{n+1}$ is injective, extends $p_n$, omits the reserved numbers, and differs finitely from $e_{\alpha_{n+1}}$.

Put $e_\alpha=\bigcup_np_n$. It is injective and omits all $k_n$, so its range is coinfinite. For each $\beta<\alpha$, choose $n$ with $\beta\le\alpha_n$. The restriction $e_\alpha\upharpoonright\beta$ is $p_n\upharpoonright\beta$, which differs finitely from $e_{\alpha_n}\upharpoonright\beta$, and hence from $e_\beta$. [Transfinite recursion](../../../../../../../transfinite-recursion.md) now gives

$$
\boxed{e_\alpha:\alpha\hookrightarrow\omega,\qquad
e_\alpha\upharpoonright\beta=^*e_\beta\quad(\beta<\alpha<\omega_1).}
$$

These [coherent coinfinite injections into omega](../../../../../../../coherent-coinfinite-injections-into-omega.md) solve the requested problem. Reserving infinitely many omitted values is important: a union of [injections](../../../../../../../injective-function.md) with individually coinfinite ranges need not itself have coinfinite range.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Iv](../../iv.md)
3. [6](../../../6.md)
4. [Paper 19](../../../../paper-19-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
