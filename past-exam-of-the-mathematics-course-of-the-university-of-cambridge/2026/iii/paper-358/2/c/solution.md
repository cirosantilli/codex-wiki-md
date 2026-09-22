<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $H_0=-d^2/dx^2+x^2$. The Hermite expansion gives

$$
\langle H_0f,f\rangle
=\sum_{m=n+1}^\infty(2m+1)|c_m|^2
=\|f'\|^2+\|xf\|^2.
$$

Since $T=-d^2/dx^2+ix^2$,

$$
\langle Tf,f\rangle=\|f'\|^2+i\|xf\|^2,
$$

and therefore

$$
\boxed{\langle Tf,f\rangle
=(i-1)\|xf\|^2
+\sum_{m=n+1}^\infty(2m+1)|c_m|^2}.
$$

Write $X=\|xf\|^2$ and $S=\sum_{m=n+1}^\infty(2m+1)|c_m|^2$. Then $\operatorname{Re}\langle Tf,f\rangle=S-X$, $\operatorname{Im}\langle Tf,f\rangle=X$, and

$$
\operatorname{Re}\langle Tf,f\rangle
+\operatorname{Im}\langle Tf,f\rangle=S\geq2n+3.
$$

If $|z|\leq n$, then $|\operatorname{Re}z+\operatorname{Im}z|\leq\sqrt2n<2n+3$, so

$$
\boxed{|z|\leq n\Longrightarrow z\notin W(Q_nTQ_n^*)}.
$$

Every fixed compact set is eventually excluded from the tail numerical ranges. Part (b) therefore implies

$$
\boxed{W_e(T)=\varnothing}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
