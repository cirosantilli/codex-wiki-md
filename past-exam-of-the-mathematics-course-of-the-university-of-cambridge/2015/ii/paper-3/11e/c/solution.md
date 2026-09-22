<h1 id="11e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume first $\beta>0$ and $d\geq0$. The nonnegative [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are

$$
O=(0,0),\qquad U=(1,0),\qquad I=(0,1-d)\quad(d\leq1),
$$

and, when both coordinates are nonnegative,

$$
C=\left(\frac{d(1+\beta)-\beta}{\beta^2},\frac{\beta-d}{\beta^2}\right).
$$

The [Jacobian matrix](../../../../../../jacobian-matrix.md) at $O$ has eigenvalues $1,1-d$, so $O$ cannot attract an initially positive uninfected population. At $U$ the eigenvalues are $-1,\beta-d$. At $I$, for $d<1$, they are $d(1+\beta)-\beta$ and $-(1-d)$. At an interior $C$, the equilibrium equations reduce the [Jacobian matrix](../../../../../../jacobian-matrix.md) to

$$
\begin{pmatrix}-x_*&-(1+\beta)x_*\\-(1-\beta)y_*&-y_*\end{pmatrix},\quad \operatorname{tr}J=-x_*-y_*<0,\quad\det J=\beta^2x_*y_*>0.
$$

Thus the coexistence equilibrium is [asymptotically stable](../../../../../../asymptotic-stability.md) precisely when $\beta/(1+\beta)<d<\beta$.

For positive initial populations these local results identify the global outcome. The relation $\dot N=N(1-N)-dy$ bounds all trajectories. With the [Dulac function](../../../../../../dulac-function.md) $1/(xy)$, the divergence of the rescaled vector field is $-1/y-1/x<0$, excluding interior periodic orbits. Boundary saddles cannot attract an interior trajectory except at the merging thresholds. The resulting **long-term outcomes** are

$$
\boxed{\begin{aligned}
0\leq d<\beta/(1+\beta)&:\ I\ \hbox{(all infected)},\\
\beta/(1+\beta)<d<\beta&:\ C\ \hbox{(coexistence)},\\
d>\beta&:\ U\ \hbox{(disease disappears)}.
\end{aligned}}
$$

At $d=\beta/(1+\beta)$, $C$ merges into $I$; at $d=\beta$, it merges into $U$. The merged equilibria still attract interior trajectories, but convergence along the zero-eigenvalue direction is algebraic. For example at $d=\beta$, put $x=1+u$, $y=v$. The local [centre manifold](../../../../../../center-manifold.md) has $u=-(1+\beta)v+O(v^2)$, and $\dot v=-\beta^2v^2+O(v^3)$. At the other threshold, using $y=(1-d)+v$, $x=u$, gives $v=(\beta-1)u+O(u^2)$ and $\dot u=-\beta^2u^2+O(u^3)$.

The invariant axes also matter: $y=0$ leads to $U$ whenever $x(0)>0$; $x=0$ leads to $I$ for $d<1$ and to extinction for $d\geq1$. At $d=1$, $I$ coincides with $O$. If $\beta=0$, disease declines for $d>0$ and any initially positive $x$ tends to $U$. If also $d=0$, every point $x+y=1$ is an equilibrium and the initial population proportions are preserved.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11E](../../11e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
