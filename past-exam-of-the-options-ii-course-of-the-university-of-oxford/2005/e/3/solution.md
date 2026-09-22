<h1 id="e/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [product topology](../../../../product-topology.md) on $X\times Y$ has the [open](../../../../open-set.md) rectangles $U\times V$, with $U$ [open](../../../../open-set.md) in $X$ and $V$ [open](../../../../open-set.md) in $Y$, as a [topological basis](../../../../basis-of-a-topology.md). The projection preimages are $p_X^{-1}(U)=U\times Y$ and $p_Y^{-1}(V)=X\times V$, so both projections are [continuous](../../../../continuous-function.md).

If $f:Z\to X\times Y$ is [continuous](../../../../continuous-function.md), both coordinate compositions are [continuous](../../../../continuous-function.md). Conversely, if both are [continuous](../../../../continuous-function.md), then

$$
f^{-1}(U\times V)=(p_X\circ f)^{-1}(U)\cap(p_Y\circ f)^{-1}(V)
$$

is [open](../../../../open-set.md) for every basic rectangle, proving [continuity](../../../../continuous-function.md) of $f$. Given [paths](../../../../continuous-path.md) between two chosen endpoints in each factor, their coordinatewise pair is therefore a [continuous path](../../../../continuous-path.md) in the product, proving that a product of [path-connected spaces](../../../../path-connected-space.md) is [path-connected](../../../../path-connected-space.md).

For the compact-neighborhood assertion, fix $x\in K$. For each $y\in L$, choose an [open](../../../../open-set.md) rectangle $U_y\times V_y$ containing $(x,y)$ inside $W$. [Compactness](../../../../compact-space.md) of $L$ chooses finitely many $V_{y_j}$ covering $L$. Put

$$
U_x=\bigcap_jU_{y_j},\qquad V_x=\bigcup_jV_{y_j}.
$$

Then $x\in U_x$, $L\subseteq V_x$, and $U_x\times V_x\subseteq W$: any point of $V_x$ belongs to one of those rectangles' second factors, while $U_x$ lies in every first factor.

[Compactness](../../../../compact-space.md) of $K$ now selects finitely many $U_{x_i}$ covering $K$. [Set](../../../../set-split.md)

$$
U=\bigcup_iU_{x_i},\qquad V=\bigcap_iV_{x_i}.
$$

These are [open](../../../../open-set.md), contain $K$ and $L$, and if $(u,v)\in U\times V$, choose an $i$ with $u\in U_{x_i}$ and use $v\in V_{x_i}$. Hence

$$
\boxed{K\times L\subseteq U\times V\subseteq W.}
$$

If $K$ or $L$ is empty, take the corresponding [open](../../../../open-set.md) factor empty and the other factor the whole space; the assertions then hold directly. No [Hausdorff](../../../../hausdorff-space.md) assumption on the factors is needed.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [E](../../e.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
