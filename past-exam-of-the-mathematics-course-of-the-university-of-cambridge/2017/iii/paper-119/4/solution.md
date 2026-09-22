<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [monad](../../../../../monad.md) on $\mathcal C$ is an endofunctor $T$ with [natural transformations](../../../../../natural-transformation.md) $\eta:1\to T$ and $\mu:T^2\to T$ satisfying

$$
\mu\,T\mu=\mu\,\mu T,\qquad \mu\,T\eta=1_T=\mu\,\eta T.
$$

An [algebra for a monad](../../../../../algebra-for-a-monad.md) is $(A,\alpha:TA\to A)$ with $\alpha\eta_A=1_A$ and $\alpha T\alpha=\alpha\mu_A$. A [morphism of algebras for a monad](../../../../../morphism-of-algebras-for-a-monad.md) $f:(A,\alpha)\to(B,\beta)$ satisfies $f\alpha=\beta Tf$. These form the [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md) $\mathcal C^T$. Its [free algebra functor](../../../../../free-algebra-functor.md) is $FX=(TX,\mu_X)$, and its [adjunction](../../../../../adjoint-functors.md) to the forgetful [functor](../../../../../functor.md) $U$ has the explicit bijection

$$
\mathcal C^T(FX,(C,\gamma))\cong\mathcal C(X,C),\qquad
h\longmapsto h\eta_X,\qquad u\longmapsto\gamma Tu.
$$

Write $S=A+B$, $V=TA+TB$, and let $\nu_1,\nu_2$ be the [coproduct in a category](../../../../../coproduct.md) injections. Set

$$
r=F(\alpha+\beta),\qquad s=\mu_SF\kappa: FV\rightrightarrows FS,
\qquad \kappa=[T\nu_1,T\nu_2].
$$

Here $\mu_S:FTS\to FS$ is an algebra [morphism](../../../../../morphism.md), with underlying multiplication $T^2S\to TS$. For an algebra $(C,\gamma)$, an algebra [morphism](../../../../../morphism.md) $h:FS\to(C,\gamma)$ corresponds to $u:S\to C$, and the transposes of $hr,hs$ are respectively

$$
u(\alpha+\beta),\qquad h\kappa=\gamma Tu\,\kappa.
$$

For the second formula, $(\mu_ST\kappa)\eta_V=\kappa$ by [naturality](../../../../../naturality.md) of $\eta$ and the [monad](../../../../../monad.md) unit law. Thus $hr=hs$ exactly when, writing $u=[a,b]$,

$$
a\alpha=\gamma Ta,\qquad b\beta=\gamma Tb.
$$

These say precisely that $a$ and $b$ are [morphisms of algebras for a monad](../../../../../morphism-of-algebras-for-a-monad.md). Consequently any [coequalizer](../../../../../coequalizer.md) $q:FS\to Q$ of $r,s$ represents pairs of algebra [morphisms](../../../../../morphism.md) out of $(A,\alpha)$ and $(B,\beta)$, proving the [coproduct presentation for monad algebras](../../../../../coproduct-presentation-for-monad-algebras.md):

$$
\boxed{Q\cong(A,\alpha)+(B,\beta)\quad\text{in }\mathcal C^T.}
$$

Its two algebra injections have underlying [morphisms](../../../../../morphism.md) $q\eta_S\nu_1$ and $q\eta_S\nu_2$; the equivalence just proved verifies both the algebra equations and their universal property.

The displayed pair is a [reflexive pair](../../../../../reflexive-pair.md), with common section

$$
t=F(\eta_A+\eta_B):FS\to FV.
$$

Indeed $rt=1_{FS}$ by the algebra unit laws, while

$$
\kappa(\eta_A+\eta_B)=\eta_S,\qquad st=\mu_SF\eta_S=1_{FS}.
$$

Now suppose $\mathcal C$ has all finite [colimits](../../../../../colimit.md) and $T$ preserves [reflexive coequalizers](../../../../../reflexive-coequalizer.md). The permitted creation theorem gives [reflexive coequalizers](../../../../../reflexive-coequalizer.md) in $\mathcal C^T$: the underlying pair is reflexive and its [coequalizer](../../../../../coequalizer.md) exists and is preserved by $T$. The preceding construction therefore gives binary algebra [coproducts in a category](../../../../../coproduct.md). The [initial object](../../../../../initial-object.md) is $F0$, since the [free algebra functor](../../../../../free-algebra-functor.md) is a [left adjoint](../../../../../adjoint-functors.md) and $0$ is initial in $\mathcal C$.

For any algebra pair $a,b:X\rightrightarrows Y$, the augmented pair

$$
[a,1_Y],[b,1_Y]:X+Y\rightrightarrows Y
$$

is a [reflexive pair](../../../../../reflexive-pair.md), with common section the injection of $Y$, and has exactly the same coequalizing [morphisms](../../../../../morphism.md) as $a,b$. Hence all [coequalizers](../../../../../coequalizer.md) exist in $\mathcal C^T$. The [construction of finite colimits from coproducts and reflexive coequalizers](../../../../../construction-of-finite-colimits-from-coproducts-and-reflexive-coequalizers.md) now gives

$$
\boxed{\mathcal C^T\text{ has all finite colimits}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
