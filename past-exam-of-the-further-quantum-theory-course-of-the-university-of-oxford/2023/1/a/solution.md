<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [irreducible spin representation](../../../../irreducible-spin-representation.md) is a nonzero [Hilbert space](../../../../hilbert-space-split.md) with no proper nonzero closed [invariant subspace](../../../../invariant-subspace.md) under all three [angular momentum operators](../../../../angular-momentum-operator-split.md). Equivalently, the associated [unitary representation](../../../../unitary-representation.md) of [SU(2)](../../../../su-2-group.md) cannot be decomposed into two nonzero orthogonal invariant pieces. The irreducible possibilities are labelled by a [spin](../../../../spin.md) $j\in\{0,\tfrac12,1,\tfrac32,\ldots\}$ and have [dimension](../../../../dimension-vector-space.md) $2j+1$.

Choose an [orthonormal basis](../../../../orthonormal-basis.md) $|j,m_s\rangle$, with $m_s=-j,-j+1,\ldots,j$. The [angular momentum commutation relations](../../../../angular-momentum-commutation-relations.md) imply $[\mathbf S^2,S_i]=0$, $[S_3,S_\pm]=\pm\hbar S_\pm$, $[S_+,S_-]=2\hbar S_3$, and $S_+^\dagger=S_-$. The complete action is

$$
\boxed{\begin{aligned}
\mathbf S^2|j,m_s\rangle&=\hbar^2j(j+1)|j,m_s\rangle,\\
S_3|j,m_s\rangle&=\hbar m_s|j,m_s\rangle,\\
S_\pm|j,m_s\rangle&=\hbar\sqrt{(j\mp m_s)(j\pm m_s+1)}\,|j,m_s\pm1\rangle.
\end{aligned}}
$$

In particular, the [spin raising operator](../../../../spin-raising-operator.md) annihilates $|j,j\rangle$ and the [spin lowering operator](../../../../spin-lowering-operator.md) annihilates $|j,-j\rangle$. The coefficient follows by taking the squared [norm](../../../../norm.md) and using $S_\mp S_\pm=\mathbf S^2-S_3^2\mp\hbar S_3$. Thus the [ladder operators](../../../../ladder-operator.md) connect every member of the [basis](../../../../basis.md), while terminating at its two endpoints.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
