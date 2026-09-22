<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

The term $p$ represents prey reproduction and $-p^2/a$ limits growth by available food, giving carrying capacity $a$ in the absence of hunters. The loss $-ph/a$ represents encounters between prey and hunters. For hunters, $hp/(8b)$ is prey-supported growth and $-h/8$ is mortality; their per-capita growth changes sign at prey population $b$. The coordinate axes are invariant, and positive initial populations remain positive.

For $a=1$, the physical [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are the origin, $(1,0)$, and $(b,1-b)$ when $b<1$. The [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J(p,h)=\begin{pmatrix}
1-2p-h&-p\\h/(8b)&(p/b-1)/8
\end{pmatrix}.
$$

At $(0,0)$ its [eigenvalues](../../../../../eigenvalue.md) are $1$ and $-1/8$, so the origin is always a [saddle equilibrium](../../../../../saddle-equilibrium.md), attracting along the hunter-only axis and repelling along the prey-only axis. At $(1,0)$ the [eigenvalues](../../../../../eigenvalue.md) are

$$
-1,\qquad\frac{1-b}{8b}.
$$

It is a [saddle equilibrium](../../../../../saddle-equilibrium.md) for $0<b<1/2$ and an asymptotically [stable node](../../../../../stable-node.md) for $b>1$.

For $0<b<1/2$, the coexistence [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J_* =\begin{pmatrix}-b&-b\\(1-b)/(8b)&0\end{pmatrix},
\qquad\lambda^2+b\lambda+\frac{1-b}{8}=0.
$$

Its [trace](../../../../../matrix-trace.md) is negative and [determinant](../../../../../determinant.md) positive. Its discriminant $b^2-(1-b)/2=(2b-1)(b+1)/2$ is negative, so **$(b,1-b)$ is an asymptotically [stable focus](../../../../../stable-spiral.md)**. Interior trajectories approach it in damped, counterclockwise oscillations in the $(p,h)$ plane. Both populations ultimately coexist.

To justify the global interior fate for this [logistic predator-prey model](../../../../../logistic-predator-prey-model.md), let $h_*=1-b$ and use the [Lyapunov function](../../../../../lyapunov-function.md)

$$
V=p-b-b\log(p/b)+8b\bigl[h-h_*-h_*\log(h/h_*)\bigr].
$$

It is nonnegative and its sublevel sets are compact inside the positive quadrant. Differentiation gives the explicit cancellation

$$
\dot V=(p-b)(1-p-h)+(h-h_*)(p-b)=-(p-b)^2.
$$

The only invariant subset on which this vanishes is $p=b,h=h_*$: remaining at $p=b$ requires $\dot p=b(1-b-h)=0$. [LaSalle's invariance principle](../../../../../lasalle-s-invariance-principle.md) therefore proves that every strictly positive initial state converges to this coexistence point.

For $b>1$, the formal coexistence point has negative $h$ and is outside the physical state space. The only physical [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md) are the [saddle equilibrium](../../../../../saddle-equilibrium.md) at the origin and the stable prey-only node. Since $\dot p\le p(1-p)$, positive prey has $\limsup p\le1$. Eventually $p<b$ with a fixed margin, so hunter population decays exponentially. When $h$ is sufficiently small, comparison with $\dot p=p(1-\varepsilon-p)$ gives $\liminf p\ge1-\varepsilon$ for every $\varepsilon>0$. Thus **$h\to0$ and $p\to1$** for positive initial prey: hunters die out and prey reaches carrying capacity.

On the boundary, hunter-only initial data approach the origin; prey-only positive data approach $(1,0)$ in either parameter range. The sketches show representative values in the two requested ranges. Dashed and dotted lines are the prey and hunter [nullclines](../../../../../nullcline.md); filled dots are attractors and open dots are [saddle equilibria](../../../../../saddle-equilibrium.md).

<a id="8b/image-predator-prey-phase-portraits-showing-stable-coexistence-for-b-0-25-and-hunter-extinction-for-b-1-5"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-2-population-portraits.png)

**[Figure 2](#8b/image-predator-prey-phase-portraits-showing-stable-coexistence-for-b-0-25-and-hunter-extinction-for-b-1-5). Predator-prey phase portraits showing stable coexistence for b=0.25 and hunter extinction for b=1.5**.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
