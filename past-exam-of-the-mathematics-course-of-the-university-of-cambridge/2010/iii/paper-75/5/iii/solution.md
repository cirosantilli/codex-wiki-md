<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [geometric embedding](../../../../../../geometric-embedding.md) means $f_*$ is [full and faithful](../../../../../../full-and-faithful-functor.md), equivalently that the adjunction counit $f^*f_*H\to H$ is invertible for every $H$. At $c$, the explicit right-adjoint formula identifies this counit with

$$
\operatorname{Nat}(\mathbb D(T-,Tc),H)\longrightarrow
\operatorname{Nat}(\mathbb C(-,c),H)\cong H(c),
$$

induced by $\tau_c:\mathbb C(-,c)\to\mathbb D(T-,Tc)$, sending $h$ to $Th$.

If $T$ is [full and faithful](../../../../../../full-and-faithful-functor.md), every $\tau_c$ is an isomorphism, making all these counit components bijective and hence making $f_*$ full and faithful. Conversely, if precomposition with $\tau_c$ is a bijection for every $H$, then $\tau_c$ is invertible by the [Yoneda lemma](../../../../../../yoneda-lemma.md) applied in the presheaf category: taking $H=\mathbb C(-,c)$ gives a left inverse, and injectivity for $H=\mathbb D(T-,Tc)$ makes it a right inverse too. Evaluating $\tau_c$ at $c'$ therefore says that

$$
\mathbb C(c',c)\xrightarrow{T}\mathbb D(Tc',Tc)
$$

is bijective for all $c,c'$. This proves the [full-faithfulness criterion for presheaf geometric embeddings](../../../../../../full-faithfulness-criterion-for-presheaf-geometric-embeddings.md):

$$
\boxed{f\text{ is an injection}\Longleftrightarrow T\text{ is full and faithful}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
