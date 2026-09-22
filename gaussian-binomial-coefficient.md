# Gaussian binomial coefficient

↑ **Parent:** [Binomial coefficient](binomial-coefficient.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_binomial_coefficient)

A [Gaussian binomial coefficient](gaussian-binomial-coefficient.md) refines an ordinary [binomial coefficient](binomial-coefficient.md) into a [polynomial](polynomial-split.md) that remembers a size statistic. For [nonnegative integers](natural-number.md) $n$ and $0\leq k\leq n$, write

$$
G_{n,k}(t)=\binom nk_t=\prod_{j=1}^k\frac{1-t^{n-k+j}}{1-t^j}.
$$

The product represents a [polynomial](polynomial-split.md); it is not an instruction to divide by zero when $t=1$ or a denominator vanishes. The [Gaussian binomial coefficient recurrence](gaussian-binomial-coefficient-recurrence.md) gives a way to compute it with only [addition](addition.md) and [multiplication](multiplication.md). The [empty product](empty-product.md) for $k=0$ is one, and $G_{n,n}(t)=1$ as well. Setting $t=1$ after obtaining the [polynomial](polynomial-split.md) recovers $\binom nk$.

For example,

$$
\boxed{G_{4,2}(t)=1+t+2t^2+t^3+t^4.}
$$

At $t=1$ this gives six objects, but its [coefficients](coefficient.md) reveal how those six objects are distributed across sizes $0,1,2,3,4$: there are two of size two and one of each other size. The [lattice-path interpretation of Gaussian binomial coefficients](lattice-path-interpretation-of-gaussian-binomial-coefficients.md) makes that information visible. Take unit steps north or east from $(0,0)$ to $(2,2)$. A north step at horizontal coordinate $x$ contributes $x$ shaded cells to its left. The six step words have total shaded [areas](surface-area.md) $0,1,2,2,3,4$.

<a id="image-the-six-lattice-paths-counted-by-g-4-2-t-weighted-by-the-number-of-shaded-cells"></a>
![](gaussian-binomial-paths-and-partitions.png)

**[Figure 18](#image-the-six-lattice-paths-counted-by-g-4-2-t-weighted-by-the-number-of-shaded-cells). The six lattice paths counted by $G_{4,2}(t)$, weighted by the number of shaded cells**. Original exact enumeration of paths with two north and two east steps. Reading shaded row lengths from top to bottom gives a [partition in a rectangle](partition-in-a-rectangle.md). Equal-sized diagrams contribute to the same [coefficient](coefficient.md).

This is useful because an aggregate count can hide the feature one actually wants. A [generating function](generating-function.md) retains the distribution of a statistic, so [coefficient extraction](coefficient-extraction.md) answers questions such as “how many allowed diagrams contain exactly two cells?” The [partition interpretation of Gaussian binomial coefficients](partition-interpretation-of-gaussian-binomial-coefficients.md) makes every [coefficient](coefficient.md) a nonnegative [integer](integer.md) without relying on cancellation in the product formula.

An unexpected second use comes from [linear algebra](linear-algebra-split.md). If $q$ is a [prime power](prime-power.md), the value $G_{n,k}(q)$ counts the $k$-dimensional [vector subspaces](vector-subspace.md) of $\mathbb F_q^n$. Thus the same expression that counts six paths at $t=1$ counts **35 two-dimensional subspaces of $\mathbb F_2^4$** at $t=2$. The [Gaussian binomial coefficient counts finite-field subspaces](gaussian-binomial-coefficient-counts-finite-field-subspaces.md) article explains why selecting a [vector subspace](vector-subspace.md) differs from selecting a [subset](subset.md) of coordinates. [Enumerative Combinatorics, Volume 1 (second-edition draft) by Richard Stanley](enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley.md)

This relationship illustrates a [q-analogue](q-analogue.md): the parameter can encode a statistic in one interpretation and the size of a [finite field](finite-field.md) in another. Here $t$ denotes the formal variable, while $q$ denotes a [finite field](finite-field.md)'s cardinality when we evaluate the [polynomial](polynomial-split.md). The interpretation using a [finite field](finite-field.md) requires $q$ to be a [prime power](prime-power.md); evaluating the [polynomial](polynomial-split.md) at an arbitrary number does not construct a field of that size.

**Table of contents**

- [Gaussian binomial coefficient recurrence](gaussian-binomial-coefficient-recurrence.md)
- [Lattice-path interpretation of Gaussian binomial coefficients](lattice-path-interpretation-of-gaussian-binomial-coefficients.md)
- [Partition interpretation of Gaussian binomial coefficients](partition-interpretation-of-gaussian-binomial-coefficients.md)
  - [Complement symmetry of Gaussian binomial coefficients](complement-symmetry-of-gaussian-binomial-coefficients.md)
- [Gaussian binomial coefficient counts finite-field subspaces](gaussian-binomial-coefficient-counts-finite-field-subspaces.md)
- [Unimodality of Gaussian binomial coefficients](unimodality-of-gaussian-binomial-coefficients.md)
- [Symmetric quantum binomial coefficient](symmetric-quantum-binomial-coefficient.md)

## ↑ Ancestors (5)

1. [Binomial coefficient](binomial-coefficient.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-5/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-4/5/ii/solution.md)
- [Q-analogue](q-analogue.md)
- [Reduced row echelon form](reduced-row-echelon-form.md)
- [Symmetric quantum binomial coefficient](symmetric-quantum-binomial-coefficient.md)
- [Unimodality of Gaussian binomial coefficients](unimodality-of-gaussian-binomial-coefficients.md)
