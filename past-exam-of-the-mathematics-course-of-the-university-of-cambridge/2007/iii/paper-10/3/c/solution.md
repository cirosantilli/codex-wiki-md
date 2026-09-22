<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The real [matrix](../../../../../../matrix.md) $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ with [determinant](../../../../../../determinant.md) one preserves $u\wedge v$. Hence $W_g(u)=W(gu)$ obeys the same [Weyl relations](../../../../../../weyl-relations.md). It is strongly continuous and irreducible because $g$ is invertible and its arguments range over the whole plane. Part (b) gives a unitary $V$ intertwining $W$ and $W_g$, so **$VW(u)V^*=W(gu)$**. If $V_1,V_2$ both work, $V_2^*V_1$ commutes with all $W$ and is scalar by part (a); its scalar has modulus one. Thus the implementer is unique up to phase.

For the displayed quarter-turn, choose the scaled inverse [Fourier transform](../../../../../../fourier-transform.md)

$$
\boxed{(Vf)(s)=\pi^{-1/2}\int_{\mathbb R}e^{2ist}f(t)\,dt.}
$$

The formula starts on [Schwartz functions](../../../../../../schwartz-function.md) and extends unitarily to $L^2$ by Plancherel and a change of scale. It conjugates $T_xf(t)=f(t+x)$ to multiplication by $e^{-2ixs}$, and multiplication by $e^{2iyt}$ to $T_y$. Keeping the Weyl phase therefore gives $VW(x,y)V^*=W(y,-x)$, as required. With the opposite Fourier-kernel sign one obtains the opposite quarter-turn, so that convention must be checked.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
