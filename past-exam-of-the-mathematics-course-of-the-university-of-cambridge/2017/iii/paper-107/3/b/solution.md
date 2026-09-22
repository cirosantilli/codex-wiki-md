<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $L=\Delta+c$ with real $c$, and let

$$
N=\{z\in C^{2,\alpha}(\overline\Omega):Lz=0,\ z|_{\partial\Omega}=0\}.
$$

The [Fredholm alternative for an elliptic Dirichlet problem](../../../../../../fredholm-alternative-for-an-elliptic-dirichlet-problem.md) says that $N$ is finite-dimensional. If $N=0$, all the prescribed data admit a unique solution. In general the exact [boundary compatibility in the self-adjoint Fredholm alternative](../../../../../../boundary-compatibility-in-the-self-adjoint-fredholm-alternative.md) is

$$
\boxed{\int_\Omega fz\,dx+\int_{\partial\Omega}\psi\,\partial_\nu z\,dS=0
\quad\text{for every }z\in N.}
$$

These conditions are necessary and sufficient; when they hold, all solutions form $u_0+N$. Thus in the second branch some data are incompatible, while compatible data have nonunique solutions. The outward [normal derivative](../../../../../../normal-derivative.md) fixes the displayed sign.

To prove the alternative, put $X=\{w\in C^{2,\alpha}(\overline\Omega):w|_{\partial\Omega}=0\}$ and $Y=C^{0,\alpha}(\overline\Omega)$. The standard zero-boundary [Poisson equation](../../../../../../poisson-equation.md) theorem makes $\Delta:X\to Y$ an isomorphism. Multiplication by $c$, followed by $\Delta^{-1}$, is a [compact operator](../../../../../../compact-operator-split.md) $K:X\to X$: the embedding $C^{2,\alpha}\hookrightarrow C^{0,\alpha}$ is compact, and multiplication is bounded. Writing $u=\psi+w$ gives

$$
(I+K)w=\Delta^{-1}F,\qquad F=f-\Delta\psi-c\psi.
$$

The [Fredholm alternative for a compact operator](../../../../../../fredholm-alternative.md) implies finite kernel and cokernel of equal dimension, and invertibility exactly when the kernel vanishes.

For the explicit compatibility conditions, use the [self-adjoint](../../../../../../self-adjoint-operator.md) Dirichlet realization of $L$ on $L^2$. It has compact resolvent: a sufficiently large positive shift of $-L$ is [coercive](../../../../../../coercive-bilinear-form.md), its inverse gains two derivatives, and the [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md) makes that inverse compact. The [Fredholm solvability condition for a self-adjoint operator](../../../../../../fredholm-solvability-condition-for-a-self-adjoint-operator.md) is $F\perp N$. Standard boundary [elliptic regularity](../../../../../../elliptic-regularity.md) upgrades the resulting [weak solution](../../../../../../weak-solution.md) to $C^{2,\alpha}$ for these data and boundary. Thus it gives the same kernel and solvability as the preceding Hölder-space formulation.

Finally [Green second identity](../../../../../../green-second-identity.md), with $z=0$ on the boundary and $Lz=0$, gives

$$
\int_\Omega zL\psi\,dx=-\int_{\partial\Omega}\psi\partial_\nu z\,dS.
$$

Consequently $\int zF=\int zf+\int\psi\partial_\nu z$, proving both necessity and sufficiency with the stated sign. If using complex data and real $c$, replace $z$ by $\overline z$ in the pairings.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
