<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Form the [HNN extension](../../../../../../hnn-extension.md) which centralizes $L$:

$$
\boxed{G_{\mathcal M}=\langle K_{\mathcal M},k\mid k^{-1}tk=t,\quad
k^{-1}r_i k=r_i,\quad k^{-1}\ell_jk=\ell_j\rangle.}
$$

This is the extension associated to the identity [isomorphism](../../../../../../isomorphism.md) $L\to L$; relations on the displayed finite generating set imply $k^{-1}hk=h$ for all $h\in L$. Since $K_{\mathcal M}$ is finitely presented and $I,J$ are finite, this is a [finite group presentation](../../../../../../finite-group-presentation.md).

For any $g\in K_{\mathcal M}$,

$$
k^{-1}gk=g\text{ in }G_{\mathcal M}\iff g\in L.
$$

The forward implication follows from [Britton's lemma](../../../../../../britton-s-lemma.md): if $g\notin L$, the word $k^{-1}gkg^{-1}$ is reduced with two stable letters and cannot be the identity. The reverse implication is the defining centralization relation. Consequently the computable word

$$
W(r,s)=k^{-1}t(r,s)k\,t(r,s)^{-1}
$$

satisfies

$$
\boxed{W(r,s)=1\text{ in }G_{\mathcal M}\iff(r,s)\in H_0(\mathcal M).}
$$

An algorithm for the [word problem for a group](../../../../../../word-problem-for-groups.md) $G_{\mathcal M}$ would therefore decide the nonrecursive set $H_0(\mathcal M)$, a contradiction. Hence $\boxed{G_{\mathcal M}\text{ has unsolvable word problem}}$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
