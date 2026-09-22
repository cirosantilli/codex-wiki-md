# Exponential generating function

↑ **Parent:** [Generating function](generating-function.md)

An [exponential generating function](exponential-generating-function.md) encodes a [sequence](sequence.md) using $A(z)=\sum_{n\geq0}a_nz^n/n!$. For labelled counting, $a_n$ is the number of structures on a fixed [set](set-split.md) of $n$ distinct labels. Labels distinguish otherwise similar objects: changing which person belongs to a group can change the structure. Recover the count by [coefficient extraction](coefficient-extraction.md) as $a_n=n![z^n]A(z)$. The raw [coefficient](coefficient.md) is $a_n/n!$, not $a_n$.

The [factorial](factorial.md) makes [multiplication](multiplication.md) account automatically for distributing labels. To combine an $A$-structure on $k$ labels and a $B$-structure on the remaining $n-k$, choose the first label [subset](subset.md) in $\binom nk$ ways, then choose the two structures. The [binomial coefficient](binomial-coefficient-split.md) counts how the two groups of labels interleave within the full label [set](set-split.md). Thus

$$
A(z)B(z)=\sum_{n\geq0}c_n\frac{z^n}{n!},\qquad c_n=\sum_{k=0}^n\binom nk a_kb_{n-k}.
$$

The normalization works because $1/(k!(n-k)!)=\binom nk/n!$. This explains the usefulness of [exponential generating functions](exponential-generating-function.md) for labelled counting: an ordinary [Cauchy product](cauchy-product.md) would omit the choices of labels. See [Peter Magyar, Math 482, notes for 2/7, labelled product principle](https://users.math.msu.edu/users/magyarp/Math482/Old.html).

For a concrete example, there is one undecorated [set](set-split.md) on any given collection of labels. Its [exponential generating function](exponential-generating-function.md) is the [exponential function](exponential-function.md) $E(z)=e^z=\sum_{n\geq0}z^n/n!$. Combine a red [set](set-split.md) and a blue [set](set-split.md), allowing either to be empty:

$$
E(z)E(z)=e^{2z}=\sum_{n\geq0}2^n\frac{z^n}{n!}.
$$

Every label independently receives one of two colours, giving $2^n$ assignments by the [rule of product](rule-of-product.md). With three labels, the counts by number of red labels are $1,3,3,1$, totalling eight. Choosing only the two group sizes would give the four possibilities $(0,3),(1,2),(2,1),(3,0)$; it would forget which labels are red.

Indeed, the [ordinary generating function](ordinary-generating-function.md) for the constant [sequence](sequence.md) $a_n=1$ is the [geometric series](geometric-series.md) $1/(1-z)$. Its square has [coefficient](coefficient.md) $[z^n](1-z)^{-2}=n+1$, counting pairs of nonnegative sizes. Both encodings are correct for their respective questions. The decision is whether identity matters when objects are combined.

For unordered [sets](set-split.md) of labelled components of positive size, an [exponential generating function](exponential-generating-function.md) $B(z)$ becomes $e^{B(z)}$: the term $B(z)^m/m!$ forgets the ordering of $m$ components. The existing [rooted-tree generating function](rooted-tree-generating-function.md) develops the richer example $T=ze^T$. A labelled [rooted tree](rooted-tree.md) consists of its [root of a tree](root-of-a-tree.md) and an unordered [set](set-split.md) of smaller labelled [rooted trees](rooted-tree.md), connecting the same label-distribution mechanism to recursive counting.

**Table of contents**

- [EGF coefficient](egf-coefficient.md)

## ↑ Ancestors (8)

1. [Generating function](generating-function.md)
2. [Power series](power-series.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Bernoulli number](bernoulli-number-split.md)
- [Bernoulli polynomial](bernoulli-polynomial.md)
- [Exponential generating function](exponential-generating-function.md)
- [Generating function](generating-function.md)
- [Labelled combinatorial structure](labelled-combinatorial-structure.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/9/b/iii/solution.md)
- [Rooted-tree generating function](rooted-tree-generating-function.md)
