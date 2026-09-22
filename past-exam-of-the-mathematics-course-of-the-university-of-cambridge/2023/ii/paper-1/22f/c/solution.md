<h1 id="22f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $T_v=T(v)$. We prove that $T$ has a closed graph. Suppose

$$
v_n\longrightarrow v\quad\text{in }V,
\qquad
T_{v_n}\longrightarrow f\quad\text{in }V^*.
$$

Put $u_n=v_n-v$ and $g=f-T_v$. Then $u_n\to0$ and $T_{u_n}\to g$ in $V^*$.

Fix $w\in V$ and $t\in\mathbb R$. Positivity and linearity give

$$
\begin{aligned}
0&\leq T_{u_n+tw}(u_n+tw)\\
 &=T_{u_n}(u_n)
 +t\bigl(T_{u_n}(w)+T_w(u_n)\bigr)
 +t^2T_w(w).
\end{aligned}
$$

Because $(T_{u_n})$ converges in the [continuous dual space](../../../../../../continuous-dual-space-split.md), its norms are bounded, so

$$
|T_{u_n}(u_n)|\leq\lVert T_{u_n}\rVert\lVert u_n\rVert\longrightarrow0.
$$

Also $T_{u_n}(w)\to g(w)$, while $T_w(u_n)\to0$ because the fixed functional $T_w$ is continuous. Passing to the limit yields

$$
0\leq t g(w)+t^2T_w(w)
$$

for every real $t$. If $g(w)\ne0$, a sufficiently small $t$ of the opposite sign makes the right-hand side negative. Hence $g(w)=0$ for every $w$, so $g=0$ and $f=T_v$.

The graph is therefore closed. The [closed graph theorem](../../../../../../closed-graph-theorem.md) now proves that $T:V\to V^*$ is continuous. This is precisely [continuity of a positive linear map into a dual space](../../../../../../continuity-of-a-positive-linear-map-into-a-dual-space.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
