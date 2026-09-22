<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [simply connected](../../../../../simply-connected-space.md) manifold is connected and orientable: its [orientation](../../../../../orientation-of-a-simplex.md) character is a [group homomorphism](../../../../../group-homomorphism.md) $\pi_1(X)\to\{\pm1\}$, and this group is trivial. Choose an [orientation](../../../../../orientation-of-a-simplex.md). The [Hurewicz theorem](../../../../../hurewicz-theorem.md) in degree one gives $H_1(X;\mathbb Z)=0$. The [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) then gives $H^1(X;\mathbb Z)=0$ and

$$
H^2(X;\mathbb Z)\cong\operatorname{Hom}(H_2(X;\mathbb Z),\mathbb Z),
$$

because the possible $\operatorname{Ext}(H_1(X),\mathbb Z)$ term is zero.

The [homology groups](../../../../../homology-group.md) are finitely generated for a closed manifold. The displayed dual group is therefore free abelian. [Poincare duality](../../../../../poincare-duality.md) identifies $H_2(X;\mathbb Z)$ with $H^2(X;\mathbb Z)$, so $H_2$ itself has no torsion. Since the second [Betti number](../../../../../betti-number.md) is one, both groups are isomorphic to $\mathbb Z$. This torsion argument is essential: rank one by itself would not rule out finite summands.

Again by [Poincare duality](../../../../../poincare-duality.md), $H^3(X;\mathbb Z)\cong H_1(X;\mathbb Z)=0$, and $H^4(X;\mathbb Z)\cong H_0(X;\mathbb Z)=\mathbb Z$. Thus the only nonzero [cohomology groups](../../../../../cohomology-group.md) are $\mathbb Z$ in degrees $0,2,4$.

Let $u$ generate $H^2$. The integral [intersection form](../../../../../intersection-form.md)

$$
Q(a,b)=\langle a\smile b,[X]\rangle
$$

is unimodular. Indeed, cap product with $[X]$ is the [Poincare duality](../../../../../poincare-duality.md) isomorphism to $H_2$, and the preceding universal-coefficient identification makes evaluation the full integral dual. Composing these isomorphisms identifies the pairing with an isomorphism $H^2\to\operatorname{Hom}(H^2,\mathbb Z)$. In rank one its matrix must therefore be $[1]$ or $[-1]$. Consequently $\langle u^2,[X]\rangle=\pm1$, so $u^2$ generates $H^4$.

All products in degrees above four vanish. Hence the assignment of the degree-two generator gives

$$
\boxed{H^*(X;\mathbb Z)\cong\mathbb Z[u]/(u^3),\qquad |u|=2,}
$$

which is the [cohomology ring of complex projective space](../../../../../cohomology-ring-of-complex-projective-space.md) for $\mathbb{CP}^2$. If the intersection form is negative, this ring isomorphism reverses the chosen top [orientation](../../../../../orientation-of-a-simplex.md) generator; preserving that additional [orientation](../../../../../orientation-of-a-simplex.md) is not part of the requested ring isomorphism.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
