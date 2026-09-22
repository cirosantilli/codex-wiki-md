<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the standard intended reading that the added edges form a [perfect matching](../../../../../../perfect-matching.md) between $G_n$ and $H_n$, the claim follows as follows. Degrees in $M_n$ remain bounded in terms of $\Delta$. For $A\subseteq V(M_n)$, write $A_G=A\cap V(G_n)$ and $A_H=A\cap V(H_n)$. The matching contributes at least $\bigl||A_G|-|A_H|\bigr|$ boundary edges, while expansion inside $G_n$ contributes a constant multiple of $\min\{|A_G|,n-|A_G|\}$. A case split according as $|A_G|\leq n/2$ or $|A_G|>n/2$ shows

$$
|\partial_{M_n}A|\geq c_{\alpha,\Delta}
\min\{|A|,2n-|A|\}.
$$

Thus $M_n$ has a uniform [Cheeger constant](../../../../../../cheeger-constant.md). [Cheeger inequality](../../../../../../cheeger-inequality.md) gives a uniformly bounded relaxation time, while $\pi_{\min}\asymp1/n$. The usual spectral mixing estimate, or part (b), then gives $t_{\mathrm{mix}}\lesssim\log n$.

If “adding $n$ edges” permits all $G_n$ vertices to attach to the same vertex of $H_n$, the assertion is false as written. Take $H_n$ to be a path and attach every vertex of the expander to one endpoint. A walk started at the other endpoint needs order $n^2$ time to reach the attachment endpoint, so its mixing time is not $O(\log n)$. The perfect-matching interpretation is therefore necessary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
