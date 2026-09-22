<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Jacobian matrix](../../../../../../jacobian-matrix.md) at a diagonal [steady state](../../../../../../steady-state.md) is

$$
J(z)=\frac1\tau\begin{pmatrix}-1&g'(z)\\g'(z)&-1\end{pmatrix},\qquad
 g'(z)=\frac{2ma^2\sigma^2z}{(\sigma^2+a^2z^2)^2}.
$$

Its [eigenvectors](../../../../../../eigenvector.md) $(1,1)$ and $(1,-1)$ represent common and opposing perturbations, with respective [eigenvalues](../../../../../../eigenvalue.md) $(-1+g')/\tau$ and $(-1-g')/\tau$.

For a nonzero equilibrium, $\sigma^2+a^2z^2=ma^2z$ and $\sigma^2/a^2=z(m-z)$. Consequently $g'(z)=2(m-z)/m$. The lower root has $g'>1$ and is a [saddle equilibrium](../../../../../../saddle-equilibrium.md); the upper root has $0<g'<1$ and is a [stable node](../../../../../../stable-node.md). At the origin $g'(0)=0$, so both [eigenvalues](../../../../../../eigenvalue.md) are $-1/\tau$.

The supplied parameters give $\sigma/a=4$, and the nonzero roots solve $z^2-10z+16=0$, giving $2$ and $8$. The numerical stability results are

$$
\boxed{\begin{array}{c|cc|c}
(x,y)&\lambda_{(1,1)}&\lambda_{(1,-1)}&\text{type}\\\hline
(0,0)&-0.1&-0.1&\text{stable node}\\
(2,2)&0.06&-0.26&\text{saddle}\\
(8,8)&-0.06&-0.14&\text{stable node}
\end{array}}
$$

Biologically, the origin is a quiescent state and the upper equilibrium a sustained mutually reinforced activity state. The saddle represents a collective activation threshold: a perturbation crossing its basin boundary can switch the network from low to high activity. This persistent-state mechanism can model a memory or decision variable, but the simplified rate equations do not establish that a particular biological circuit uses it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
