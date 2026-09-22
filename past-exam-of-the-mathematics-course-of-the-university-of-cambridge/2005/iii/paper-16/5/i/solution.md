<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here is an alternative route for the ergodicity step using the [Birkhoff ergodic theorem](../../../../../../birkhoff-ergodic-theorem.md). After invariance has been proved, the theorem identifies the almost-everywhere limit of $A_n\varphi$ with $\mathbb E_\mu[\varphi\mid\mathcal I]$. The hypothesis therefore gives

$$
\mathbb E_\mu[\varphi\mid\mathcal I]=\int\varphi\,d\mu
$$

for every [continuous function](../../../../../../continuous-function.md) $\varphi$. For an invariant [Borel set](../../../../../../borel-set.md) $B$, approximate $h=\mathbf1_B$ in $L^1$ by such a $\varphi$. Since $h$ is measurable with respect to the [invariant sigma-algebra](../../../../../../invariant-sigma-algebra.md), its [conditional expectation](../../../../../../conditional-expectation.md) is $h$ itself. The [L1 contraction of conditional expectation](../../../../../../l1-contraction-of-conditional-expectation.md) gives

$$
\left\|h-\mu(B)\right\|_1
\leq\left\|\mathbb E_\mu[h-\varphi\mid\mathcal I]\right\|_1
 +\left|\int(\varphi-h)\,d\mu\right|
\leq2\|h-\varphi\|_1.
$$

Arbitrarily accurate continuous approximation forces $h=\mu(B)$ almost everywhere. Thus this use of the theorem reaches the same zero-or-one criterion as the direct averaging proof above, without assuming in advance that $\mu$ is [ergodic](../../../../../../ergodicity.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
