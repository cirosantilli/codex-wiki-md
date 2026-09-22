<h1 id="11i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\beta(s)=(\beta_1(s),\beta_2(s))$, $\gamma(t)=(\gamma_1(t),\gamma_2(t))$, and

$$
h(s,t)=\beta(s)-\gamma(t).
$$

The endpoint conditions imply

$$
\begin{array}{ll}
h_1(s,-1)\geq0,&h_1(s,1)\leq0,\\
h_2(-1,t)\leq0,&h_2(1,t)\geq0.
\end{array}
$$

Let $P(x)=\max(-1,\min(1,x))$ and define the continuous self-map of $I^2$

$$
F(s,t)=\bigl(P(s-h_2(s,t)),\ P(t+h_1(s,t))\bigr).
$$

By Brouwer, $F$ has a fixed point $(s,t)$. If $s$ is interior, its fixed-point equation gives $h_2=0$. At $s=-1$ or $s=1$, the projection equation and the corresponding displayed boundary sign again force $h_2=0$. The identical argument in the second coordinate gives $h_1=0$. Hence

$$
h(s,t)=0,
$$

so

$$
\boxed{\beta(s)=\gamma(t).}
$$

The two paths intersect.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11I](../../11i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
