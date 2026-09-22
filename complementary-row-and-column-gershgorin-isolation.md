# Complementary row and column Gershgorin isolation

↑ **Parent:** [Gershgorin eigenvalue counting](gershgorin-eigenvalue-counting.md)

A [matrix](matrix.md) and its [transpose](transpose.md) have the same [characteristic polynomial](characteristic-polynomial.md), allowing two independent [Gershgorin eigenvalue counting](gershgorin-eigenvalue-counting.md) arguments for one [spectrum](spectrum-functional-analysis.md). If isolated row discs certify simple [eigenvalues](eigenvalue.md) near one group of centres and isolated column discs certify the remaining ones, pairwise separation of all the certified small discs establishes a simple spectrum even if neither full family has pairwise disjoint discs.

For example, let $n=2m$, the diagonal centres be $1,\ldots,n$, and all adjacent off-diagonal entries have magnitude strictly below $1/4$. Add a corner entry $a_{n1}=c$. The row radii are below $1/4,1/2,\ldots,1/2,|c|+1/4$; the column radii reverse the two endpoint bounds. If $|c|\leq m-3/4$, rows isolate centres $1,\ldots,m$ and columns isolate centres $m+1,\ldots,n$. The nearest potentially enlarged-disc contact has centre separation $m$, while the radius sum is strictly less than $|c|+3/4\leq m$. Each of the $n$ certified small discs contains one simple [eigenvalue](eigenvalue.md). For real entries these [eigenvalues](eigenvalue.md) are real, since a nonreal conjugate pair would put two roots in the same conjugation-invariant isolated disc.

This is a sufficient uniform certificate. Overlap beyond this bound does not prove repeated [eigenvalues](eigenvalue.md); individual [matrices](matrix.md) can have simple real spectra well beyond a [Gershgorin disc](gershgorin-disc.md) separation bound.

## ↑ Ancestors (7)

1. [Gershgorin eigenvalue counting](gershgorin-eigenvalue-counting.md)
2. [Gershgorin circle theorem](gershgorin-circle-theorem.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/3/e/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2007/p/p4/f/solution.md)
