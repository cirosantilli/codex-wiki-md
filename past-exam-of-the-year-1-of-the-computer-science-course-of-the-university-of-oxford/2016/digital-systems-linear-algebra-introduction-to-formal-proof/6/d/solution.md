<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Interpret “distinct [eigenvalues](../../../../../eigenvalue.md)” as **$n$ pairwise distinct [eigenvalues](../../../../../eigenvalue.md) in the chosen [field](../../../../../field.md)**. Select a nonzero [eigenvector](../../../../../eigenvector.md) $z_i$ for each. A single nonzero [vector](../../../../../vector.md) is [linearly independent](../../../../../linear-independence.md). Suppose inductively that $z_1,\ldots,z_k$ are [linearly independent](../../../../../linear-independence.md). If adding $z_{k+1}$ made the set [linearly dependent](../../../../../linear-dependence.md), its nontrivial relation would have a nonzero coefficient of $z_{k+1}$, since otherwise it would contradict the induction hypothesis. Solving for $z_{k+1}$ would place it in the [linear span](../../../../../linear-span.md) of the first $k$ [eigenvectors](../../../../../eigenvector.md).

Part (c) would then force $\lambda_{k+1}=\lambda_i$ for some $i\leq k$, contradicting pairwise distinctness. [Mathematical induction](../../../../../mathematical-induction.md) therefore proves that **all $n$ selected [eigenvectors](../../../../../eigenvector.md) are [linearly independent](../../../../../linear-independence.md)**, forming a [basis](../../../../../basis.md). If the [field](../../../../../field.md) is $\mathbb R$, the assertion requires $n$ real [eigenvalues](../../../../../eigenvalue.md); a real [matrix](../../../../../matrix.md) can instead have nonreal [eigenvalues](../../../../../eigenvalue.md) and a [eigenvector](../../../../../eigenvector.md) basis over the [complex numbers](../../../../../complex-number.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
