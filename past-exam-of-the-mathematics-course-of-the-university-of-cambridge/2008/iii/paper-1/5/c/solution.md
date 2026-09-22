<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same intended [weak-star topology](../../../../../../weak-star-topology.md) as in (b), and assume $C\ne\varnothing$. The induced operator is $T=S^*$, so $T\phi(x)=\phi(Sx)$; it is weak-star continuous because evaluation after applying $T$ is still evaluation at a [vector](../../../../../../vector.md) of $E$.

Choose $\phi\in C$ and form the averages

$$
\phi_n=\frac1n\sum_{j=0}^{n-1}T^j\phi.
$$

Invariance and convexity put every $\phi_n$ in $C$. Weak-star closedness and (b) make $C$ compact, so some subsequence converges to $\psi\in C$. Telescoping gives

$$
T\phi_n-\phi_n=\frac{T^n\phi-\phi}{n},\qquad
\|T\phi_n-\phi_n\|\leq\frac2n,
$$

because both orbit points lie in the dual [unit ball](../../../../../../unit-ball.md). Weak-star [continuity](../../../../../../continuous-function.md) now gives $T\psi-\psi=0$. Hence $\boxed{T\text{ has a fixed point in }C.}$ This is the [weak-star fixed point theorem for an adjoint operator](../../../../../../weak-star-fixed-point-theorem-for-an-adjoint-operator.md); it does not require $T$ to be a contraction on the entire [dual space](../../../../../../dual-space.md).

If “weakly closed” is interpreted literally as closed for $\sigma(E^*,E^{**})$, the result can fail. Take $E=c_0$, let $S$ be the left shift and $T=S^*$ the right shift on $\ell^1$. The set

$$
C=\{x\in\ell^1:x_j\geq0,\ \sum_jx_j=1\}
$$

is a nonempty weakly closed convex subset of the [unit ball](../../../../../../unit-ball.md): its defining coordinate inequalities and sum equality are weakly closed. It is invariant under the right shift. But a fixed [vector](../../../../../../vector.md) of that shift has first coordinate zero and then every coordinate zero, so none belongs to $C$. This supplies a counterexample to the literal topology and explains why the weak-star qualification is essential.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
