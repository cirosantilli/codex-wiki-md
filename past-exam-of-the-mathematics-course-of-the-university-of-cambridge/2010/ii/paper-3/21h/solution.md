<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

The real [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) states that if $X$ is compact Hausdorff and $A\subseteq C(X,\mathbb R)$ is a [subalgebra](../../../../../subalgebra.md) containing the constants and separating points, then $A$ is uniformly dense in $C(X,\mathbb R)$. Let $B$ be its uniform closure, still an [algebra over a field](../../../../../algebra-over-a-field.md). If $h\in B$ and $M\ge\|h\|_\infty$, scale the permitted [polynomial](../../../../../polynomial-split.md) approximation of absolute value on $[-1,1]$ to $[-M,M]$. Applying these [polynomials](../../../../../polynomial-split.md) to $h$ proves $|h|\in B$. Therefore

$$
\max(h,k)=\tfrac12(h+k+|h-k|),\qquad
\min(h,k)=\tfrac12(h+k-|h-k|)
$$

belong to $B$: it is a lattice.

Fix $f\in C(X,\mathbb R)$ and $\varepsilon>0$. For every $x,y\in X$, point separation and an affine adjustment give $g_{x,y}\in A$ with $g_{x,y}(x)=f(x)$ and $g_{x,y}(y)=f(y)$; if $x=y$, a constant suffices. For fixed $x$, the open sets where $g_{x,y}>f-\varepsilon$ cover $X$. Select finitely many and take their maximum $h_x\in B$. Then $h_x>f-\varepsilon$ everywhere and $h_x(x)=f(x)$. By [continuity](../../../../../continuous-function.md), $h_x<f+\varepsilon$ on some neighborhood $V_x$ of $x$. Choose finitely many $V_x$ covering $X$ and take the minimum of the corresponding $h_x$. The result $h\in B$ satisfies $f-\varepsilon<h<f+\varepsilon$ everywhere. Since $B$ is closed and $\varepsilon$ arbitrary, $f\in B$. Thus **$\overline A=C(X,\mathbb R)$**, proving the theorem.

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
