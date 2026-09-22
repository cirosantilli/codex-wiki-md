<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [monad](../../../../../../monad.md) $(T,\eta,\mu)$, an [algebra for a monad](../../../../../../algebra-for-a-monad.md) is $(A,a:TA\to A)$ with $a\eta_A=1_A$ and $aT(a)=a\mu_A$. A [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md) $f:(A,a)\to(B,b)$ satisfies $fa=bTf$. These objects and arrows form the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) $\mathcal C^T$.

The [free algebra functor](../../../../../../free-algebra-functor.md) sends $A$ to $(TA,\mu_A)$ and $f$ to $Tf$. The monad identities verify the algebra laws. For the forgetful [functor](../../../../../../functor.md) $U$, the free adjunction is

$$
\mathcal C^T((TA,\mu_A),(B,b))\cong\mathcal C(A,B),\qquad h\mapsto h\eta_A,
$$

with inverse $v\mapsto bTv$. The algebra law makes the latter an [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md). The identities $h\eta_A\mapsto bT(h\eta_A)=h\mu_AT\eta_A=h$ and $bTv\eta_A=b\eta_Bv=v$ prove the [bijection](../../../../../../bijection.md).

In the [category of adjunctions inducing a fixed monad](../../../../../../category-of-adjunctions-inducing-a-fixed-monad.md), objects are adjunctions $F\dashv G$ with their induced monad identified with $T$. A [morphism](../../../../../../morphism.md) to $F'\dashv G'$ is a [functor](../../../../../../functor.md) $H$ between the right-hand [categories](../../../../../../category-split.md) satisfying $G'H=G$, $HF=F'$ and compatibility with units and counits. With these strict identifications, define

$$
K(B)=(GB,G\varepsilon_B),\qquad K(f)=Gf.
$$

The triangle identities give the unit algebra law; naturality of $\varepsilon$ at $\varepsilon_B$ gives the multiplication law. Naturality at $f$ makes $Gf$ an [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md). Moreover $UK=G$, $KF=F^T$ because $G\varepsilon_{FA}=\mu_A$, and $K\varepsilon_B$ is the free-adjunction counit at $K(B)$. Hence $K$ is a [morphism](../../../../../../morphism.md) into the Eilenberg-Moore adjunction.

For any other such $H$, its underlying object at $B$ must be $GB$. Counit compatibility forces its algebra action to be $G\varepsilon_B$, and the forgetful [functor](../../../../../../functor.md), which is a [faithful functor](../../../../../../faithful-functor.md), forces $H(f)=Gf$. Thus $H=K$. This proves [terminality of the Eilenberg-Moore adjunction](../../../../../../terminality-of-the-eilenberg-moore-adjunction.md). If adjunctions are specified only up to coherent [isomorphisms](../../../../../../isomorphism.md), the same argument gives uniqueness up to the corresponding compatible [natural isomorphism](../../../../../../natural-isomorphism.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
