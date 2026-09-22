<h1 id="1/iii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove (b)$\Rightarrow$(a) by induction on dimension, using the independently proved (c)$\Rightarrow$(a) argument in the next section. Work on an integral [projective variety](../../../../../../../projective-variety.md) $V$ of dimension $d>0$. The hypothesis is inherited by all its integral closed [subvarieties](../../../../../../../closed-subvariety.md). Induction therefore makes $D$ [ample](../../../../../../../ample-line-bundle.md) on every strictly lower-dimensional closed reduced [subvariety](../../../../../../../closed-subvariety.md), and hence on every proper closed subscheme of dimension less than $d$, by [ampleness on reduced components](../../../../../../../ampleness-on-reduced-components.md).

Choose an [effective Cartier divisor](../../../../../../../effective-cartier-divisor.md) $H$ which is a [very ample](../../../../../../../very-ample-line-bundle.md) hyperplane section of $V$. Then $\mathcal O_H(D)$ is [ample](../../../../../../../ample-line-bundle.md). We need a vanishing statement uniform in extra positive $H$-twists:

$$
H^j(H,\mathcal O_H(mD+tH))=0\qquad(j>0,\ m\ge M,\ t\ge0).
$$

Here is a justification using [Castelnuovo–Mumford regularity](../../../../../../../castelnuovo-mumford-regularity.md). Embed $H$ by $\mathcal O_H(H)$. For each of the finitely many positive cohomology degrees $j$, [Serre vanishing](../../../../../../../serre-vanishing.md) for the [ample](../../../../../../../ample-line-bundle.md) bundle $\mathcal O_H(D)$ makes $H^j(H,\mathcal O_H(mD-jH))$ vanish for $m\ge M$. Thus the pushed-forward sheaf $\mathcal O_H(mD)$ is zero-regular. Persistence of regularity makes it $t+j$-regular for every $t\ge0$, giving exactly the displayed vanishing. This is the [uniform Serre vanishing for two ample twists](../../../../../../../uniform-serre-vanishing-for-two-ample-twists.md) lemma. It does not assume that $D$ is [ample](../../../../../../../ample-line-bundle.md) on $V$.

Apply the [divisor restriction exact sequence](../../../../../../../divisor-restriction-exact-sequence.md) to $H$ with twists $mD+tH$. For $i\ge2$, both neighbouring cohomology groups on $H$ vanish, so

$$
H^i(V,\mathcal O_V(mD+tH))\cong H^i(V,\mathcal O_V(mD+(t+1)H))\qquad(t\ge0).
$$

For a fixed $m\ge M$, sufficiently large $t$ kills the right-hand cohomology by [Serre vanishing](../../../../../../../serre-vanishing.md) for $H$ on $V$. The [higher cohomology vanishing from an ample hyperplane restriction](../../../../../../../higher-cohomology-vanishing-from-an-ample-hyperplane-restriction.md) argument gives $H^i(V,\mathcal O_V(mD))=0$ for all $i\ge2$. Consequently

$$
h^0(V,mD)=\chi(V,mD)+h^1(V,mD)\ge\chi(V,mD)\longrightarrow\infty.
$$

This step is essential: divergence of a polynomial does not by itself prove that its top-degree coefficient is positive.

For $m$ large enough, $h^0(V,mD)>1$. Evaluation at a closed point has a one-dimensional target, so its kernel contains a nonzero section vanishing there. We have obtained condition (c) on $V$. Lower-dimensional [subvarieties](../../../../../../../closed-subvariety.md) already have the same property by induction, so the next section's implication (c)$\Rightarrow$(a) applies. Thus

$$
\boxed{\text{(b)}\Longrightarrow\text{(a)}}.
$$

For $d=1$, higher groups with $i\ge2$ vanish automatically and the same evaluation argument starts the induction. The regularity facts used above are stated in [the Stacks Project, regularity lemmas](https://stacks.math.columbia.edu/tag/08A2).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iii](../../iii.md)
3. [1](../../../1.md)
4. [Paper 134](../../../../paper-134-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
