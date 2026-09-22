<h1 id="26i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After a fixed orthogonal change of ambient coordinates, a neighbourhood of $p$ in $X$ is the graph

$$
\{(u,g(u)):u\in U\subseteq\mathbb R^d\}
$$

of a smooth map $g:U\to\mathbb R^{n-d}$. Write $p_i=(u_i,g(u_i))$ for all sufficiently large $i$. Every tangent vector has the unique form

$$
w_i=(v_i,Dg(u_i)v_i).
$$

The convergence of $w_i$ implies convergence of its first component, say $v_i\to v$. Since $u_i\to u$ and $Dg$ is continuous,

$$
w_i\longrightarrow(v,Dg(u)v)\in T_pX.
$$

This proves the [closedness of tangent spaces under convergent base points](../../../../../../closedness-of-tangent-spaces-under-convergent-base-points.md).

Conversely, suppose $d>0$ and write $w=(v,Dg(u)v)\in T_pX$. Choose a nonzero $e\in\mathbb R^d$ and positive $t_i\to0$ with $u_i=u+t_ie\in U$. Then

$$
p_i=(u_i,g(u_i))\ne p,
\qquad
w_i=(v,Dg(u_i)v)\in T_{p_i}X,
$$

and $p_i\to p$, $w_i\to w$. **Every tangent vector arises as such a limit from distinct base points.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26I](../../26i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
