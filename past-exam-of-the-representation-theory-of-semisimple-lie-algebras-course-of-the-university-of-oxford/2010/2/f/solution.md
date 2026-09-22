<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the standard defining properties of [Category O](../../../../category-o.md): finite generation over $U(\mathfrak g)$, a [direct sum](../../../../direct-sum.md) of finite-dimensional [weight spaces](../../../../weight-space.md), and locally finite [positive root](../../../../positive-root.md) action. In particular the weights lie in a finite union of downward [root](../../../../root-of-a-root-system.md) cones. Submodules and quotients retain the [representation weight](../../../../weight-of-a-representation.md) bounds and finite [weight spaces](../../../../weight-space.md); finite generation of submodules follows from the [Poincaré-Birkhoff-Witt theorem](../../../../poincare-birkhoff-witt-theorem.md) and the noetherian property of $U(\mathfrak g)$.

Choose finitely many [weight vector](../../../../weight-vector.md) generators. The sum $T$ of their full [weight spaces](../../../../weight-space.md) is finite-dimensional and preserved by the centre. The [kernel](../../../../kernel-of-a-linear-map-split.md) of its central action has finite codimension in $Z(U(\mathfrak g))$ and kills the generators, hence, by centrality, all of $M$. Thus only finitely many central characters $\theta_1,\ldots,\theta_r$ can occur in any subquotient: they are the characters of a fixed finite-dimensional commutative [quotient](../../../../quotient.md) algebra of the centre.

By the [Harish-Chandra isomorphism](../../../../harish-chandra-isomorphism.md) each $\theta_i$ determines one finite Weyl orbit of shifted weights. Let $S$ be the finite union of these orbits after subtracting $\rho$. Every nonzero subquotient has a nonzero highest-[weight vector](../../../../weight-vector.md), using the bounded-above weights. Within its finite-dimensional [highest weight](../../../../highest-weight-of-a-representation.md) space, the commuting central operators have a common [eigenvector](../../../../eigenvector.md). Part (e) and the central-character restriction show that its [highest weight](../../../../highest-weight-of-a-representation.md) belongs to $S$.

Define for any subquotient $N$

$$
d(N)=\sum_{\nu\in S}\dim N_\nu.
$$

It is finite, additive in short exact sequences, and positive whenever $N\ne0$. Hence each strict step of a [submodule](../../../../submodule.md) chain consumes at least one unit of $d(M)$. Refining a nonsimple factor into a proper [submodule](../../../../submodule.md) and [quotient](../../../../quotient.md) cannot continue more than $d(M)$ times. It ends with simple factors, proving

$$
\boxed{M\text{ has a composition series of finite length, at most }d(M).}
$$

The argument proves the assertion for every object of $\mathcal O$, rather than just for a cyclic [highest weight](../../../../highest-weight-of-a-representation.md) object.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the representation theory of semisimple Lie algebras course of the University of Oxford](../../../split.md)
5. [Representation theory of semisimple Lie algebras course of the University of Oxford](../../../../representation-theory-of-semisimple-lie-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
