<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Consider the commutative square

$$
\begin{array}{ccc}
\mathcal A&\xrightarrow{H}&\mathcal C\\
\downarrow F&&\downarrow G\\
\mathcal B&\xrightarrow{K}&\mathcal D,
\end{array}
$$

where $F$ is a [final functor](../../../../../../final-functor.md) and $G$ is a [discrete fibration](../../../../../../discrete-fibration.md). For $B\in\mathcal B$, choose an object $(A,\beta:B\to FA)$ of the nonempty [comma category](../../../../../../comma-category.md) $(B\downarrow F)$. Commutativity gives an arrow

$$
K\beta:KB\longrightarrow KFA=GHA.
$$

Lift it uniquely through $G$ with codomain $HA$, and define $LB$ to be the domain of this lift.

This definition does not depend on the choice of $(A,\beta)$. A morphism $u:(A,\beta)\to(A',\beta')$ in the comma category satisfies $Fu\,\beta=\beta'$. The composite of the lift of $K\beta$ with $Hu$ is then a lift of $K\beta'$ with codomain $HA'$, so uniqueness of discrete-fibration lifts says that it is the chosen lift and has the same domain. Since $(B\downarrow F)$ is connected, all choices give the same object $LB$.

For $v:B\to B'$, define $Lv$ as the unique lift through $G$ of $Kv:KB\to KB'=G(LB')$ with codomain $LB'$. Its domain is $LB$: choose $\beta':B'\to FA$, and observe that composing this lift with the lift of $K\beta'$ yields the lift associated with $\beta'v:B\to FA$. Uniqueness of lifting also proves preservation of identities and composition, so $L$ is a functor and $GL=K$.

For $B=FA$, choose $(A,1_{FA})$ in $(FA\downarrow F)$. The lift of $1_{GHA}$ is $1_{HA}$, hence $LFA=HA$; the same lifting argument on arrows gives $LF=H$. Finally, if $L'$ is another filler, then for every $\beta:B\to FA$, the arrow $L'\beta:L'B\to HA$ is a lift of $K\beta$. Unique lifting forces $L'B=LB$ and then forces equality on arrows. Thus $L$ is unique, proving [orthogonality of final functors and discrete fibrations](../../../../../../orthogonality-of-final-functors-and-discrete-fibrations.md).

## ↑ Ancestors (11)

1. [I](../i.md)
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
