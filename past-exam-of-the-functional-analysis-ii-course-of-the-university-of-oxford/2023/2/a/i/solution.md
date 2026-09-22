<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Banach-Steinhaus convergence theorem](../../../../../banach-steinhaus-convergence-theorem.md) can be stated as follows. Let $X$ be a [normed space](../../../../../normed-vector-space-split.md), $Y$ a [Banach space](../../../../../banach-space-split.md), and $A_n\in\mathcal B(X,Y)$. If

$$
\sup_n\|A_n\|<\infty
$$

and $A_nd$ converges in $Y$ for every $d$ in a [dense subset](../../../../../dense-set.md) $D\subseteq X$, then $A_nx$ converges for every $x\in X$. The pointwise limit $A$ is a [bounded linear operator](../../../../../continuous-linear-operator.md) and

$$
\boxed{A_nx\longrightarrow Ax\quad(x\in X),\qquad\|A\|\leq\liminf_n\|A_n\|.}
$$

If $X$ is also a [Banach space](../../../../../banach-space-split.md), the uniform [operator norm](../../../../../operator-norm.md) bound is necessary: pointwise convergence implies pointwise boundedness, so the [Banach-Steinhaus theorem](../../../../../uniform-boundedness-principle.md), namely the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md), supplies it. The limit is convergence in the [strong operator topology](../../../../../strong-operator-topology.md); it need not be convergence in [operator norm](../../../../../operator-norm.md).

To see the sufficient direction, write $C=\sup_n\|A_n\|$. For $d\in D$ the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\|A_nx-A_mx\|\leq2C\|x-d\|+\|A_nd-A_md\|.
$$

First approximate $x$ by $d$, then let $m,n\to\infty$. Completeness of $Y$ gives the limit. Linearity passes to limits, and $\|Ax\|=\lim_n\|A_nx\|\leq(\liminf_n\|A_n\|)\|x\|$ gives the displayed bound. If a candidate [bounded linear operator](../../../../../continuous-linear-operator.md) $A:X\to Y$ is already given and $A_nd\to Ad$ on $D$, the same approximation proves convergence to $Ax$ even when $Y$ is merely a [normed space](../../../../../normed-vector-space-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
