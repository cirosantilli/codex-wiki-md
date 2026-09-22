<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [comma category](../../../../../comma-category.md) $(B\downarrow F)$ has objects $(A,u:B\to FA)$ and morphisms $h:(A,u)\to(A',u')$ satisfying $F(h)u=u'$. An initial object $(LB,\eta_B)$ is precisely a universal arrow from $B$ to $F$. Such choices for every $B$ define a functor $L$ and natural bijections $\mathcal C(LB,A)\cong\mathcal D(B,FA)$, hence a left [adjoint functor](../../../../../adjoint-functors.md). The unit of an existing adjunction supplies the initial objects in the reverse direction.

Suppose $F:\mathcal C\to\mathcal D$ is final and $\alpha_A:D(FA)\to X$ is a cocone. For $B\in\mathcal D$, choose $(A,u:B\to FA)$ in $(B\downarrow F)$ and define

$$
\alpha_B=\alpha_A\,D(u).
$$

Connectedness of the comma category makes this independent of the choice, and applying the same argument to arrows proves naturality. Any extension must have this value, so it is unique. Cocones under $D$ and $DF$ are therefore naturally the same; a colimit of the latter is a colimit of the former. Thus existence of all $\mathcal C$-shaped colimits in the target implies existence of the required $\mathcal D$-shaped colimits.

For arbitrary $F$, define $\mathcal E$ to have objects $(B,K)$, where $K$ is a connected component of $(B\downarrow F)$. An arrow $(B,K)\to(B',K')$ is an arrow $v:B\to B'$ whose precomposition functor sends $K'$ into $K$. Let $H(B,K)=B$, and let $G(A)=(FA,K_A)$ where $K_A$ contains $(A,1_{FA})$. Then $F=HG$. Given $v:B\to H(B',K')$, precomposition selects one and only one component $K$, yielding the unique lift $(B,K)\to(B',K')$; hence $H$ is a [discrete fibration](../../../../../discrete-fibration.md). Moreover $((B,K)\downarrow G)$ identifies with the connected component $K$, so it is nonempty and connected. Thus $G$ is a [final functor](../../../../../final-functor.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
