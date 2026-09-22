<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the fact that $K$ is a [normal subgroup](../../../../../normal-subgroup.md) to move a factor of $K$ past a factor of $H$. For $h_1,h_2\in H$ and $k_1,k_2\in K$,

$$
(h_1k_1)(h_2k_2)=h_1h_2(h_2^{-1}k_1h_2)k_2\in HK,
$$

while

$$
(hk)^{-1}=k^{-1}h^{-1}=h^{-1}(hk^{-1}h^{-1})\in HK.
$$

The [identity element](../../../../../identity-element.md) belongs to $HK$. Hence **$HK$ is a [subgroup](../../../../../subgroup.md)**, by the [subgroup test](../../../../../subgroup-test.md). This proves the [product of a subgroup with a normal subgroup](../../../../../product-of-a-subgroup-with-a-normal-subgroup.md) construction; $H$ need not be a [normal subgroup](../../../../../normal-subgroup.md).

For each $h\in H$, [conjugation](../../../../../conjugation.md) maps $K$ to itself and respects its multiplication. The inverse of $k\mapsto h^{-1}kh$ is $k\mapsto hkh^{-1}$, so both are [group automorphisms](../../../../../group-automorphism.md) of $K$.

**The printed formula requires a composition convention.** For the printed $\phi_h(k)=h^{-1}kh$, ordinary [function composition](../../../../../function-composition.md) gives

$$
\boxed{\phi_{h_1h_2}=\phi_{h_2}\circ\phi_{h_1}.}
$$

Indeed, $(h_1h_2)^{-1}k(h_1h_2)=h_2^{-1}(h_1^{-1}kh_1)h_2$. Thus the displayed assignment is a [group antihomomorphism](../../../../../group-antihomomorphism.md) with the usual multiplication in the [automorphism group](../../../../../automorphism-group.md). It is a [group homomorphism](../../../../../group-homomorphism.md) if the [automorphisms](../../../../../automorphism.md) are written as right operators and multiplied in the corresponding reverse order; this is precisely why [right conjugation reverses composition](../../../../../right-conjugation-reverses-composition.md).

With the usual left [function composition](../../../../../function-composition.md), the corresponding [group homomorphism](../../../../../group-homomorphism.md) is instead

$$
\boxed{\psi:H\longrightarrow\operatorname{Aut}(K),\qquad\psi_h(k)=hkh^{-1}.}
$$

Direct expansion gives $\psi_{h_1h_2}(k)=h_1(h_2kh_2^{-1})h_1^{-1}=(\psi_{h_1}\circ\psi_{h_2})(k)$. This states the intended [conjugation action](../../../../../conjugation-action.md) without silently reversing the order in the printed formula.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
