<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [Boolean algebra](../../../../../../boolean-algebra.md) $B$, let $U(B)$ be its set of [ultrafilters](../../../../../../ultrafilter.md), equivalently the Boolean homomorphisms $B\to2$. Regard $U(B)$ as an object of $\mathbf{Set}^{\mathrm{op}}$. A homomorphism $k:B\to B'$ acts by inverse image of ultrafilters, a set map $U(B')\to U(B)$, hence an arrow $U(B)\to U(B')$ in the opposite category.

A Boolean homomorphism $h:B\to\mathcal P(A)$ gives the function

$$
a\longmapsto\{b\in B:a\in h(b)\}\quad\text{from }A\text{ to }U(B).
$$

Conversely, a function $v:A\to U(B)$ gives $h(b)=\{a:b\in v(a)\}$. The ultrafilter laws are exactly what makes this map preserve the Boolean operations, including complements and $0,1$. These constructions are inverse and natural, proving the [Boolean ultrafilter-power-set adjunction](../../../../../../boolean-ultrafilter-power-set-adjunction.md)

$$
\boxed{U\dashv\mathcal P:\mathbf{Set}^{\mathrm{op}}\longrightarrow\mathbf{Bool}.}
$$

Its unit is $\eta_B(b)=\{u\in U(B):b\in u\}$.

Take $B=\mathcal P(\mathbb N)$, an object in the image of the right adjoint. There is a [nonprincipal ultrafilter](../../../../../../nonprincipal-ultrafilter.md) on $\mathbb N$, by extending the cofinite filter in the usual choice setting. The subset $P\subset U(B)$ consisting of all [principal ultrafilters](../../../../../../principal-ultrafilter.md) is not $\eta_B(b)$ for any $b\subseteq\mathbb N$: containing the principal ultrafilter at every integer forces $b=\mathbb N$, but $\eta_B(\mathbb N)=U(B)$ also contains the nonprincipal ultrafilters. Thus $\eta_B$ is not surjective and is not an isomorphism. By the necessary condition proved in the root solution, **this adjunction is not idempotent**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
