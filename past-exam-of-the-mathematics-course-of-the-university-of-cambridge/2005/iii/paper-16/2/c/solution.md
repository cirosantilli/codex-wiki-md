<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $x$ have a dense forward [orbit](../../../../../../orbit-dynamical-system.md) $O=\{f^j(x):j\geq0\}$, and suppose that $f$ is [surjective](../../../../../../surjective-function.md). Every tail $O_k=\{f^j(x):j\geq k\}$ is then [dense](../../../../../../dense-set.md). Indeed, [continuity](../../../../../../continuous-function.md) gives

$$
f^k(\overline O)\subseteq\overline{f^k(O)}=\overline{O_k},
$$

and the left side equals $f^k(X)=X$ by [surjectivity](../../../../../../surjective-function.md).

Given nonempty [open sets](../../../../../../open-set.md) $U,V$, choose $k\geq0$ with $f^k(x)\in U$. The dense tail $O_{k+1}$ supplies $j\geq k+1$ with $f^j(x)\in V$. Taking $n=j-k\geq1$ gives $f^j(x)\in f^n(U)\cap V$. This proves the required positive-time intersection property.

**The result can fail without [surjectivity](../../../../../../surjective-function.md).** Take the [compact metric space](../../../../../../compact-metric-space.md)

$$
X=\{0\}\cup\{1/j:j\geq1\},qquad
f(0)=0,qquad f(1/j)=1/(j+1),
$$

with the [metric](../../../../../../metric.md) induced from the [real line](../../../../../../real-line.md). All nonzero points are [isolated](../../../../../../isolated-point.md), so [continuity](../../../../../../continuous-function.md) there is automatic; at zero, $f(1/j)\to0=f(0)$ proves [continuity](../../../../../../continuous-function.md). The forward [orbit](../../../../../../orbit-dynamical-system.md) of $1$ is $\{1,1/2,1/3,\ldots\}$, whose [closure](../../../../../../closure-topology.md) is $X$, so this is [point transitivity](../../../../../../point-transitivity.md). But $f(X)=X\setminus\{1\}$. The singletons $U=\{1/2\}$ and $V=\{1\}$ are nonempty [open sets](../../../../../../open-set.md), and for every $n\geq1$,

$$
f^n(U)=\{1/(n+2)\},qquad f^n(U)\cap V=\varnothing.
$$

The isolated initial point can be visited only at the start of the dense forward [orbit](../../../../../../orbit-dynamical-system.md); deleting that initial segment destroys density.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
