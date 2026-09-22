<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No: uniform convergence of utilities on bounded sets does not imply closed convergence of preferences.** It does imply the upper condition. Indeed, suppose $x_j\to x$, $y_j\to y$ and $u_{n_j}(x_j)\geq u_{n_j}(y_j)$. These bundles all lie in one bounded ball. Uniform convergence there, together with continuity of $u$, gives

$$
u(x)=\lim_j u_{n_j}(x_j)\geq\lim_j u_{n_j}(y_j)=u(y),
$$

so $x\succeq y$.

For a strict limiting comparison $u(x)>u(y)$, the fixed pair itself satisfies $u_n(x)>u_n(y)$ eventually. The obstruction is the lower condition at an [indifference relation](../../../../../../indifference-relation.md), where the strict approximating rankings need not disappear.

For a counterexample valid in every dimension $L\geq1$, take

$$
u(x)=0,\qquad u_n(x)=\frac{x_1}{n}\quad(x\in\mathbb R_+^L).
$$

On $\|x\|\leq k$, $|u_n(x)-u(x)|\leq k/n\to0$, exactly as required. Every $u_n$ induces $x\succeq_n y$ if and only if $x_1\geq y_1$, while $u$ makes every pair indifferent. In particular, $0\succeq e_1$ holds in the limit. Any sequences $x_n\to0$, $y_n\to e_1$ eventually have $(x_n)_1<(y_n)_1$, so they cannot satisfy $x_n\succeq_n y_n$. The lower graph-limit condition fails.

Equivalently, an open neighborhood of $(0,e_1)$ sufficiently small to keep the first coordinate of its first bundle below that of its second bundle meets the limiting graph and none of the approximating graphs. The corresponding hit-open neighborhood in the [Fell topology](../../../../../../fell-topology.md) proves failure of convergence directly. Hence

$$
\boxed{\text{the upper condition always holds, but the lower condition need not hold.}}
$$

The [uniform utility convergence need not preserve closed preference convergence](../../../../../../uniform-utility-convergence-need-not-preserve-closed-preference-convergence.md) phenomenon reflects the loss of ranking information when the limiting utility has a flat indifference region.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
