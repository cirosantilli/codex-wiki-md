<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $c_{u,v}$ for [braiding](../../../../braiding.md) and $M_{u,v}=c_{v,u}c_{u,v}$ for [anyon monodromy](../../../../anyon-monodromy.md). Transparency says $M_{a,x}=1$ for every $x$. The [hexagon identities for braiding](../../../../hexagon-identity-for-braiding.md) express [braiding](../../../../braiding.md) a composite $a\otimes b$ past $x$ as successive [braidings](../../../../braiding.md) of its two factors past $x$. If $a,b$ are both [transparent anyons](../../../../transparent-anyon.md), move $x$ around $b$ and then around $a$; both full moves are identities, hence

$$
M_{a\otimes b,x}=1.
$$

This is the [fusion closure of transparent anyons](../../../../fusion-closure-of-transparent-anyons.md) at the level of the composite object.

For completeness, let $i:c\to a\otimes b$ and $p:a\otimes b\to c$ be an inclusion and projection for an allowed [anyon fusion](../../../../anyon-fusion-rule.md) summand, with $pi=1_c$. Naturality of [braiding](../../../../braiding.md) gives

$$
M_{c,x}=(p\otimes1_x)M_{a\otimes b,x}(i\otimes1_x)=1_{c\otimes x}.
$$

Thus

$$
\boxed{a,b\text{ transparent and }N^c_{ab}>0\quad\Longrightarrow\quad c\text{ transparent}.}
$$

The [vacuum anyon](../../../../vacuum-anyon.md) belongs to this collection, and taking duals preserves transparency, so it is also closed under [antianyons](../../../../antianyon.md).

There is a further restriction on the [spin of a transparent anyon](../../../../spin-of-a-transparent-anyon.md). Apply the [anyon balancing identity](../../../../anyon-balancing-identity.md) to the [vacuum anyon](../../../../vacuum-anyon.md) channel of $a\times\bar a$:

$$
1=R^{a\bar a}_1R^{\bar a a}_1=\frac{\theta_1}{\theta_a\theta_{\bar a}}=\frac1{\theta_a^2}.
$$

Here ribbon duality gives $\theta_{\bar a}=\theta_a$ and $\theta_1=1$. Consequently

$$
\boxed{\theta_a=+1\ \text{or}\ -1.}
$$

Their [topological spins](../../../../topological-spin.md) are those of [bosons](../../../../boson.md) or [fermions](../../../../fermion.md). This does not imply $d_a=1$: a [transparent anyon](../../../../transparent-anyon.md) can have several [anyon fusion](../../../../anyon-fusion-rule.md) channels, with nontrivial exchange action within them, even though every full [anyon monodromy](../../../../anyon-monodromy.md) is trivial. If the theory is additionally a [modular tensor category](../../../../modular-tensor-category.md), the only [transparent anyon](../../../../transparent-anyon.md) is the [vacuum anyon](../../../../vacuum-anyon.md); Question 1 need not impose that extra hypothesis.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the anyons and topological quantum field theories course of the University of Oxford](../../../split.md)
5. [Anyons and topological quantum field theories course of the University of Oxford](../../../../anyons-and-topological-quantum-field-theories-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
