<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes, provided “commute” means pairwise commute.** Necessity follows because three [diagonal matrices](../../../../diagonal-matrix.md) commute pairwise.

For sufficiency, first choose the common [eigenbasis](../../../../eigenbasis.md) for the first two [linear maps](../../../../linear-map.md), say $S,T$, obtained in part (b). Their joint [eigenspaces](../../../../eigenspace.md)

$$
W_{\lambda,\mu}=\ker(S-\lambda I)\cap\ker(T-\mu I)
$$

give a [direct sum](../../../../direct-sum.md) decomposition of $V$. The third map $U$ preserves each $W_{\lambda,\mu}$, since $SUv=USv=\lambda Uv$ and $TUv=UTv=\mu Uv$. By the [diagonalizable restriction lemma](../../../../diagonalizable-restriction-lemma.md), $U|_{W_{\lambda,\mu}}$ has a [basis](../../../../basis.md) of [eigenvectors](../../../../eigenvector.md) there. Every such vector already has fixed [eigenvalues](../../../../eigenvalue.md) for $S$ and $T$.

Joining these bases therefore gives **a common [eigenbasis](../../../../eigenbasis.md) for all three maps**. The same induction proves [simultaneous diagonalization](../../../../simultaneous-diagonalization.md) for any finite pairwise commuting family of [diagonalizable](../../../../diagonalizable-matrix.md) [linear endomorphisms](../../../../linear-endomorphism.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
