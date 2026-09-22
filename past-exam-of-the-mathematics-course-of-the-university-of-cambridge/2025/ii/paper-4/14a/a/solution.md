<h1 id="14a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a spatially homogeneous equilibrium of the [Brusselator](../../../../../../brusselator.md), the reaction terms obey

$$
0=\alpha-(\beta+1)u+u^2v,
\qquad
0=\beta u-u^2v.
$$

Positivity gives $uv=\beta$, and substitution into the first equation gives

$$
(u_*,v_*)=\left(\alpha,\frac\beta\alpha\right).
$$

The reaction Jacobian there is

$$
J=
\begin{pmatrix}
\beta-1&\alpha^2\\
-\beta&-\alpha^2
\end{pmatrix},
$$

so

$$
\operatorname{tr}J=\beta-1-\alpha^2<0,
\qquad
\det J=\alpha^2>0.
$$

The [linear stability analysis](../../../../../../linear-stability.md) therefore makes the equilibrium asymptotically stable. It is a stable node when

$$
(\beta-1-\alpha^2)^2\geq4\alpha^2
$$

and a stable focus when the reverse strict inequality holds. Since the upper-right entry of $J$ is positive and the lower-left entry is negative, focus trajectories rotate clockwise. Thus the local phase portrait consists of trajectories approaching the fixed point, either directly as a node or while spiralling clockwise as a focus.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14A](../../14a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
