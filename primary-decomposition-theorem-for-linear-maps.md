# Primary decomposition theorem for linear maps

↑ **Parent:** [Kernel decomposition for coprime polynomials](kernel-decomposition-for-coprime-polynomials.md)

For a [linear map](linear-map.md) $T:V\to V$ on a [finite-dimensional vector space](finite-dimensional-vector-space.md) over a [field](field.md) $F$, factor its [minimal polynomial](minimal-polynomial.md) as $m_T=\prod_i p_i^{a_i}$ with distinct [monic polynomials](monic-polynomial.md) $p_i$ that are [irreducible polynomials](irreducible-polynomial.md). Then

$$
\boxed{V=\bigoplus_i V_i,\qquad V_i=\ker p_i(T)^{a_i},\qquad m_{T|_{V_i}}=p_i^{a_i}}.
$$

Each $V_i$ is an [invariant subspace](invariant-subspace.md), since $T$ commutes with every [polynomial](polynomial-split.md) in $T$. These are canonical [vector subspaces](vector-subspace.md), determined by $T$, without requiring any [eigenvalues](eigenvalue.md) in $F$.

For a proof, put $m_i=p_i^{a_i}$ and $M_i=m_T/m_i$. The [coprime polynomials](coprime-polynomials.md) $m_i,M_i$ admit a [Bézout's identity for polynomials](bezout-s-identity-for-polynomials.md) $b_iM_i+c_im_i=1$. Set $E_i=b_i(T)M_i(T)$. Its image is contained in $V_i$ because $m_i(T)E_i=0$. The [polynomial](polynomial-split.md) $\sum_i b_iM_i-1$ is divisible by every $m_i$, hence by their product, so $\sum_iE_i=I$. On $V_i$, $E_i=I$; on $V_j$ with $j\ne i$, $E_i=0$ because $m_j$ divides $M_i$. These facts prove the [direct sum](direct-sum.md) and identify $E_i$ as its [projection operators](projection-linear-algebra.md). Finally, if the [minimal polynomial](minimal-polynomial.md) of any [restriction](restriction-mathematics.md) had a smaller exponent, $m_T/p_i$ would annihilate every summand and hence all of $V$, a contradiction.

## ↑ Ancestors (8)

1. [Kernel decomposition for coprime polynomials](kernel-decomposition-for-coprime-polynomials.md)
2. [Minimal polynomial](minimal-polynomial.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Minimal polynomial of a normal operator](minimal-polynomial-of-a-normal-operator.md)
- [Solution](past-exam-of-the-algebra-1-and-differential-equations-1-course-of-the-university-of-oxford/2015/2/b/i/solution.md)
- [Solution](past-exam-of-the-algebra-1-and-differential-equations-1-course-of-the-university-of-oxford/2015/2/b/ii/solution.md)
- [Solution](past-exam-of-the-algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford/2013/1/c/solution.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2017/2/b/ii/solution.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/1/a/i/solution.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/1/a/ii/solution.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/3/c/iii/solution.md)
