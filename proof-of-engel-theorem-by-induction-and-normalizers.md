# Proof of Engel theorem by induction and normalizers

↑ **Parent:** [Engel's theorem](engel-s-theorem.md)

First prove the [Engel lemma](engel-lemma.md) by induction on the dimension of a [Lie algebra](lie-algebra-split.md) of [nilpotent endomorphisms](nilpotent-linear-map.md). If $x^m=0$, then $\operatorname{ad}x=L_x-R_x$ on the endomorphism algebra has $(\operatorname{ad}x)^{2m-1}=0$, since left and right multiplication commute. Thus a proper [Lie subalgebra](lie-subalgebra.md) $M$ acts nilpotently on $L/M$, and induction gives a nonzero class normalized by $M$. This proves the [Engel normalizer lemma](engel-normalizer-lemma.md).

For a maximal proper $M$, its normalizer is all of $L$, so $M$ is an ideal. Maximality then forces $\dim L/M=1$, since every line in a Lie algebra is a subalgebra. Induction gives a nonzero common annihilator $W$ of $M$ in the representation space. Ideality makes $W$ stable under $L$. A generator $x$ of $L/M$ is nilpotent on $W$ and has nonzero kernel there, providing a vector killed by all of $L$. In the possibly nonfaithful quotient actions, apply induction to the image, whose dimension is at most $\dim M$.

Repeatedly apply this common-kernel statement to quotient representation spaces to obtain a complete flag with $xV_j\subseteq V_{j-1}$. Hence the operators are simultaneously strictly upper triangular. Applying this to the [Adjoint representation](adjoint-representation-of-a-lie-algebra.md) shows that a finite-dimensional [Lie algebra](lie-algebra-split.md) whose every adjoint map is nilpotent has terminating [lower central series](lower-central-series.md). Conversely, termination of that series immediately makes every adjoint map nilpotent. This proves [Engel theorem](engel-s-theorem.md).

// Target: semisimple-lie-algebra.bigb

## ↑ Ancestors (10)

1. [Engel's theorem](engel-s-theorem.md)
2. [Nilpotent Lie algebra](nilpotent-lie-algebra.md)
3. [Lower central series of a Lie algebra](lower-central-series-of-a-lie-algebra.md)
4. [Lie algebra](lie-algebra-split.md)
5. [Lie theory](lie-theory-split.md)
6. [Diagonal dominance](diagonal-dominance.md)
7. [Algebra](algebra-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2/4/solution.md)
