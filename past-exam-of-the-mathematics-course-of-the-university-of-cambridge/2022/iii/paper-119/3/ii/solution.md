<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an arbitrary functor $F:\mathcal C\to\mathcal D$, define a category $\mathcal E$ as follows. Its objects are pairs $(B,c)$, where $B\in\mathcal D$ and $c$ is a connected component of $(B\downarrow F)$. Precomposition by an arrow $g:B\to B'$ defines

$$
g^*:(B'\downarrow F)\longrightarrow(B\downarrow F).
$$

There is one morphism $(B,c)\to(B',c')$ over $g$ exactly when $g^*(c')=c$. Functoriality of precomposition makes this a category, and projection

$$
G:\mathcal E\longrightarrow\mathcal D,
\qquad G(B,c)=B,
$$

is a discrete fibration: given $g:B\to B'=G(B',c')$, its unique lift with codomain $(B',c')$ has domain $(B,g^*c')$.

Define $H:\mathcal C\to\mathcal E$ by

$$
H(A)=\bigl(FA,[1_{FA}]\bigr),
$$

where $[1_{FA}]$ is the component of the identity object in $(FA\downarrow F)$. For $u:A\to A'$, use the unique arrow over $Fu$. It exists because $(Fu)^*[1_{FA'}]$ contains the object $Fu:FA\to FA'$, and this object is joined to $1_{FA}$ by the morphism $u$ in $(FA\downarrow F)$. Plainly $GH=F$.

For $(B,c)\in\mathcal E$, an object of $((B,c)\downarrow H)$ is exactly an arrow $\beta:B\to FA$ lying in the component $c$: the condition for an arrow $(B,c)\to H(A)$ is precisely $\beta^*[1_{FA}]=c$. Morphisms agree with those in $(B\downarrow F)$. Hence

$$
((B,c)\downarrow H)\cong c,
$$

which is nonempty and connected by definition. Therefore $H$ is final. We have factored $F=GH$ as a final functor followed by a discrete fibration, giving the [final-discrete-fibration factorization](../../../../../../final-discrete-fibration-factorization.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
