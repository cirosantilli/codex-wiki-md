<h1 id="14c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Split the real contour at zero and rotate its positive part to angle $\theta\in(0,\pi/4)$ and its negative part to angle $\pi-\theta$. Rotate the two rays of $\partial D^+$ to these same angles, preserving orientation. The initial-transform pole at $k=i$ is not crossed by either real-contour rotation, while $\widehat u_0(-k)$ has its pole at $-i$, outside the upper half-plane. The apparent poles in $\widetilde g_0$ are removable.

On the rotated rays, both $\operatorname{Im}k>0$ and $\operatorname{Re}k^2>0$. The initial-data factor has Gaussian decay $|e^{ikx-k^2t}|=e^{-x\operatorname{Im}k-t\operatorname{Re}k^2}$. For the boundary term, retain the [integral](../../../../../../integral.md) form

$$
e^{-k^2t}\widetilde g_0(k^2,t)=\int_0^te^{-k^2(t-s)}\sin s\,ds,
$$

which is $O(|k|^{-2})$ there. Multiplication by $e^{ikx}$ gives exponential decay as $|k|\to\infty$ for every fixed $x>0$. Thus all integrands are exponentially damped on the deformed contours; the endpoint boundary value at $x=0$ is taken afterwards, rather than claiming uniform exponential decay there.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14C](../../14c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
