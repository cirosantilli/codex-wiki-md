<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [monad](../../../../../../monad.md) is an endofunctor $T:\mathcal C\to\mathcal C$ with [natural transformations](../../../../../../natural-transformation.md) $\eta:1_{\mathcal C}\to T$ and $\mu:T^2\to T$ satisfying

$$
\mu\,T\eta=\mu\,\eta T=1_T,\qquad \mu\,T\mu=\mu\,\mu T.
$$

Its [Kleisli category](../../../../../../kleisli-category.md) has the same objects as $\mathcal C$, with $\mathcal C_T(A,B)=\mathcal C(A,TB)$, identity $\eta_A$, and composite

$$
g\star f=\mu_C T(g)f\qquad(f:A\to TB,\ g:B\to TC).
$$

The unit laws follow from naturality of $\eta$ and the two monad unit laws. For $h:C\to TD$, the two triple composites reduce, using naturality of $\mu$, to

$$
\mu_D\mu_{TD}T^2(h)T(g)f
\quad\text{and}\quad
\mu_DT(\mu_D)T^2(h)T(g)f;
$$

they agree by the monad associativity law. Thus this is a [category](../../../../../../category-split.md).

Define the [free functor into a Kleisli category](../../../../../../free-functor-into-a-kleisli-category.md) $J$ and the right-hand [functor](../../../../../../functor.md) $U$ by

$$
JA=A,\quad J(f)=\eta_Bf,\qquad UA=TA,\quad U(f)=\mu_BT(f).
$$

The identity and composition formulas for $J$ are

$$
J(1_A)=\eta_A,\qquad
J(g)\star J(f)=\mu_CT(\eta_C)T(g)\eta_Bf=\eta_Cgf=J(gf).
$$

For $U$, $U(\eta_A)=\mu_AT\eta_A=1_{TA}$, and

$$
U(g\star f)=\mu_CT\mu_CT^2(g)T(f)
=\mu_C\mu_{TC}T^2(g)T(f)
=\mu_CT(g)\mu_BT(f)=U(g)U(f),
$$

where the last step is naturality of $\mu$. Hence both mappings are [functors](../../../../../../functor.md). The hom-set identity $\mathcal C_T(JA,B)=\mathcal C(A,UB)$ gives the [adjunction](../../../../../../adjoint-functors.md) $J\dashv U$. Its unit is $\eta$, and its counit at $B$ is the Kleisli arrow represented by $1_{TB}:TB\to TB$. Applying $U$ to that counit gives $\mu_B$, so the induced monad is the specified one.

For any $L\dashv R:\mathcal D\to\mathcal C$ inducing this same [monad](../../../../../../monad.md), with counit $\varepsilon$, define the [Kleisli comparison functor](../../../../../../kleisli-comparison-functor.md)

$$
KA=LA,\qquad K(f:A\to TB)=\varepsilon_{LB}L(f).
$$

The triangular identities give $K(\eta_A)=1_{LA}$, and naturality of the counit together with $\mu=R\varepsilon L$ gives $K(g\star f)=K(g)K(f)$. Explicitly, naturality moves $\varepsilon_{LB}$ past $L(g)$, then moves the resulting counit past $\varepsilon_{LC}$, reducing the composite to $\varepsilon_{LC}L(\mu_CT(g)f)$. Thus $K$ is a [functor](../../../../../../functor.md), with $KJ=L$ and $RK=U$, and it sends the Kleisli counit to $\varepsilon_L$.

An adjunction morphism here is required to commute with the left and right adjoints and preserve their adjunction structure. Such a morphism must have the above object map; every Kleisli arrow $f$ factors as its counit after $J(f)$, so its arrow map is forced as well. This proves [initiality of the Kleisli adjunction](../../../../../../initiality-of-the-kleisli-adjunction.md):

$$
\boxed{J\dashv U\text{ is initial among adjunctions inducing }(T,\eta,\mu).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
