# Integer partition

↑ **Parent:** [Set partition](set-partition.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integer_partition)

An [integer partition](integer-partition.md) of a [nonnegative integer](natural-number.md) $n$ is a [multiset](multiset.md) of [positive integers](positive-integer.md) whose [sum](sum.md) is $n$: repetitions matter, but the order of the summands does not. Equivalently, write its parts in decreasing order, allowing equality:

$$
\lambda=(\lambda_1,\ldots,\lambda_\ell),\qquad
\lambda_1\geq\cdots\geq\lambda_\ell>0,\qquad
\sum_{i=1}^{\ell}\lambda_i=n.
$$

The notation $\lambda\vdash n$ says that $\lambda$ is an [integer partition](integer-partition.md) of $n$. The partition count $p(n)$ counts all [integer partitions](integer-partition.md) of $n$, with any number of parts. Zero has one empty [integer partition](integer-partition.md), so $p(0)=1$. The [partition of an integer](partition-of-an-integer.md) article develops the same objects in [representation theory of the symmetric group](representation-theory-of-the-symmetric-group-split.md).[section 1.7, definitions of partitions and diagrams](enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley.md)

**Computed example.** The seven [integer partitions](integer-partition.md) of five are exactly

$$
5;\quad 4+1;\quad 3+2;\quad 3+1+1;\quad
2+2+1;\quad 2+1+1+1;\quad 1+1+1+1+1.
$$

Thus $p(5)=7$. Sorting each list of positive summands into decreasing order prevents repetitions in this enumeration. Grouping by largest part verifies completeness: largest parts $5,4,3,2,1$ contribute respectively $1,1,2,2,1$ possibilities. For largest part $3$, the remaining $2$ is either $2$ or $1+1$; for largest part $2$, the remaining $3$ uses only $2$ and $1$, giving $2+1$ or $1+1+1$.

<a id="image-all-seven-integer-partitions-of-five-drawn-as-ferrers-diagrams-each-row-has-as-many-dots-as-its-part"></a>
![](integer-partitions-of-five.png)

**[Figure 15](#image-all-seven-integer-partitions-of-five-drawn-as-ferrers-diagrams-each-row-has-as-many-dots-as-its-part). All seven integer partitions of five, drawn as Ferrers diagrams: each row has as many dots as its part**.

An [integer partition](integer-partition.md) keeps sizes without named positions. The [compositions of an integer](composition-of-an-integer.md) $(3,2)$ and $(2,3)$ are different [tuples](finite-tuple.md), but sorting either gives the same [integer partition](integer-partition.md) $3+2$. A [weak composition of an integer](weak-composition-of-an-integer.md) $(0,3,2)$ also retains its empty first position; dropping its zero and sorting gives that same [integer partition](integer-partition.md). Conversely, a [set partition](set-partition.md) records which distinct elements belong to each block. For example, the [set partitions](set-partition.md) $\{\{1,2,3\},\{4,5\}\}$ and $\{\{1,2,4\},\{3,5\}\}$ differ even though both have the same [integer partition](integer-partition.md) $3+2$ of block sizes.

The [Ferrers diagram](ferrers-diagram.md) makes an [integer partition](integer-partition.md) into a shape. For $3+2$, the column lengths are $2,2,1$: exchanging rows and columns gives its [conjugate partition](conjugate-partition.md) $2+2+1$. Exchanging again recovers $3+2$, so this operation is a [bijection](bijection.md). In particular, the three [integer partitions](integer-partition.md) of five with at most two parts are $5$, $4+1$, and $3+2$; their [conjugate partitions](conjugate-partition.md) $1+1+1+1+1$, $2+1+1+1$, and $2+2+1$ are precisely the three with largest part at most two. This visible symmetry explains the equal counts for these two restrictions. The square-cell version is the existing [Young diagram](young-diagram.md).

**Counting by a generating function.** An [integer partition](integer-partition.md) is determined by its multiplicities $m_j$, the number of parts equal to $j$. Its size condition is $\sum_{j\geq1}j m_j=n$. Consequently its [ordinary generating function](ordinary-generating-function.md) is

$$
\sum_{n\geq0}p(n)q^n
=\prod_{j\geq1}\left(1+q^j+q^{2j}+\cdots\right)
=\prod_{j\geq1}\frac{1}{1-q^j}.
$$

**Proof outline.** Choose the term $q^{jm_j}$ from the $j$th [geometric series](geometric-series.md). The product contributes $q^n$ exactly when those multiplicities describe an [integer partition](integer-partition.md) of $n$, once for each such [integer partition](integer-partition.md). As a [formal power series](formal-power-series.md), each [coefficient](coefficient.md) is determined by finitely many factors: factors with $j>n$ contribute only their constant term to the [coefficient](coefficient.md) of $q^n$. For $n=5$, multiplication through $j=5$ gives $1+q+2q^2+3q^3+5q^4+7q^5$ up to degree five, independently recovering $p(5)=7$. Restricting the factors gives the [generating function for partitions with bounded parts](generating-function-for-partitions-with-bounded-parts.md). This is useful because restrictions on summands become choices of factors, while [conjugate partitions](conjugate-partition.md) turn restrictions on numbers of rows into restrictions on row lengths.[section 1.8, conjugation and partition generating functions](enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley.md)

**Table of contents**

- [Partition in a rectangle](partition-in-a-rectangle.md)
- [Ferrers diagram](ferrers-diagram.md)

## ↑ Ancestors (5)

1. [Set partition](set-partition.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Complement symmetry of Gaussian binomial coefficients](complement-symmetry-of-gaussian-binomial-coefficients.md)
- [Composition of an integer](composition-of-an-integer.md)
- [Ferrers diagram](ferrers-diagram.md)
- [Integer partition](integer-partition.md)
- [Monomial symmetric function](monomial-symmetric-function.md)
- [Partition in a rectangle](partition-in-a-rectangle.md)
- [Partition interpretation of Gaussian binomial coefficients](partition-interpretation-of-gaussian-binomial-coefficients.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-77/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-77/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-109/1/iii/solution.md)
- [Power-sum symmetric polynomial](power-sum-symmetric-polynomial.md)
- [Schur polynomial](schur-polynomial.md)
- [Set partition](set-partition.md)
- [Stars and bars (combinatorics)](stars-and-bars-combinatorics.md)
