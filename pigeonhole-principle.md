# Pigeonhole principle

↑ **Parent:** [Combinatorics](combinatorics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pigeonhole_principle)

Place $N$ objects into $m\geq1$ boxes, assigning each object to exactly one box. Here $N$ is a nonnegative [integer](integer.md) and $m$ is a [positive integer](positive-integer.md). The [pigeonhole principle](pigeonhole-principle.md) says that if $N>m$, some box contains at least two objects. Equivalently, a [function](function-split.md) from an $N$-element [finite set](finite-set.md) to an $m$-element [finite set](finite-set.md) cannot be an [injective function](injective-function.md) when $N>m$. The boxes may stand for categories rather than physical containers. [Lehman, Leighton and Meyer, Mathematics for Computer Science, section 14.8, rule 14.8.1](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/mit6_042js15_textbook.pdf#page=581)

For thirteen objects and twelve boxes, a box containing at least two is unavoidable. Thinking of thirteen people and their birth months gives the same conclusion: at least two share a birth month. Twelve people could occupy the twelve months one apiece, so thirteen is the smallest number that forces a shared month. The [generalized pigeonhole principle](generalized-pigeonhole-principle.md) quantifies how many objects must share a box when there are still more objects.

The useful surprise is that the [pigeonhole principle](pigeonhole-principle.md) proves existence without needing to locate the objects involved. Choosing a good assignment rule is often the creative step: equal labels can mean equal remainders, nearby [points](point-geometry.md), or repeated states of an [algorithm](algorithm.md). Once the rule is chosen, a short count can force a relationship among a much larger collection of objects. The [pigeonhole principle](pigeonhole-principle.md) itself does not name the crowded box. When the objects and their assignments are explicitly available, a simple [algorithm](algorithm.md) finds one: scan the objects, keep the first object seen in each box, and stop when a later object enters an occupied box. At most $m+1$ scanned objects are needed when $N>m$.

**A geometric example.** Any five [points](point-geometry.md) in a [square](square.md) of side one contain two whose [Euclidean distance](euclidean-distance.md) is at most $1/\sqrt2$. Give each [point](point-geometry.md) [Cartesian coordinates](cartesian-coordinate-system.md) $(x,y)\in[0,1]^2$. Divide both ranges into the [intervals](interval-mathematics.md) $[0,1/2)$ and $[1/2,1]$, making four cells. Thus $x<1/2$ belongs to the left half and $x\geq1/2$ to the right half; $y<1/2$ belongs to the lower half and $y\geq1/2$ to the upper half. This convention assigns every boundary [point](point-geometry.md) to exactly one cell.

The [pigeonhole principle](pigeonhole-principle.md) puts two of the five [points](point-geometry.md) in the same cell. Their differences in [Cartesian coordinates](cartesian-coordinate-system.md) have magnitude at most $1/2$, so the [Pythagorean theorem](pythagorean-theorem.md) gives their [Euclidean distance](euclidean-distance.md) $d$ the bound

$$
d^2\leq\left(\frac12\right)^2+\left(\frac12\right)^2=\frac12,
\qquad d\leq\frac1{\sqrt2}\approx0.707107.
$$

For the plotted [points](point-geometry.md) $(0.1,0.1)$, $(0.4,0.4)$, $(0.8,0.2)$, $(0.2,0.8)$ and $(0.8,0.8)$, the first two occupy the lower-left cell and have [Euclidean distance](euclidean-distance.md) $\sqrt{0.3^2+0.3^2}=\sqrt{0.18}\approx0.424264$. These [Cartesian coordinates](cartesian-coordinate-system.md) exhibit the forced pair; the argument applies to every placement of five [points](point-geometry.md).

<a id="image-the-pigeonhole-principle-places-two-of-five-points-in-one-of-four-cells-of-a-square-bounding-their-euclidean-distance-by-1-sqrt2"></a>
![](geometric-pigeonhole-square.png)

**[Figure 1](#image-the-pigeonhole-principle-places-two-of-five-points-in-one-of-four-cells-of-a-square-bounding-their-euclidean-distance-by-1-sqrt2). The pigeonhole principle places two of five points in one of four cells of a square, bounding their Euclidean distance by $1/\sqrt2$**.

**An arithmetic example.** Assign eight [integers](integer.md) to their seven [residue classes](residue-class.md) modulo the [integer modulus](modulus-in-modular-arithmetic.md) $7$. The [pigeonhole principle](pigeonhole-principle.md) gives two with the same [residue class](residue-class.md), so $7$ is an [integer divisor](divisor.md) of their difference. In $\{2,5,9,12,16,20,24,27\}$, for example, $2$ and $9$ satisfy the [integer congruence](integer-congruence.md) $9\equiv2\pmod7$, and $9-2=7$. Likewise, assigning [fractional parts](fractional-part.md) to short [intervals](interval-mathematics.md) gives the [Dirichlet approximation theorem](dirichlet-s-approximation-theorem.md); its existing article explains the approximation bound.

**Table of contents**

- [Generalized pigeonhole principle](generalized-pigeonhole-principle.md)
- [Infinite pigeonhole principle](infinite-pigeonhole-principle.md)

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (52)

- [Alphabet insensitivity lemma](alphabet-insensitivity-lemma.md)
- [Cyclic permutation](cyclic-permutation.md)
- [Dirichlet's approximation theorem](dirichlet-s-approximation-theorem.md)
- [Divisibility chain inside a finite-sums set](divisibility-chain-inside-a-finite-sums-set.md)
- [Finite-height polynomial root avoidance](finite-height-polynomial-root-avoidance.md)
- [Finite Ramsey theorem](finite-ramsey-theorem.md)
- [Function collision](function-collision.md)
- [Hash collision](hash-collision.md)
- [Hash function](hash-function.md)
- [Multiplicity-free complete dyadic spectrum](multiplicity-free-complete-dyadic-spectrum.md)
- [Nonwrapping progression in a cyclic Bohr set](nonwrapping-progression-in-a-cyclic-bohr-set.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-10/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-25/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-12/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-27/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-13/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/7e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1/17f/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-10/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-60/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-10/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/10f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/10f/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/13e/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-108/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-130/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/12g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/17i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-130/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/17g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-130/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-130/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-129/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-130/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-166/1/a/solution.md)
- [Pigeonhole principle](pigeonhole-principle.md)
- [Polynomial-length progression in a dense triple sumset](polynomial-length-progression-in-a-dense-triple-sumset.md)
- [Second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md)
- [Siegel's lemma](siegel-s-lemma.md)
- [Six-vertex monochromatic triangle argument](six-vertex-monochromatic-triangle-argument.md)
- [Unit-ideal identity for powers](unit-ideal-identity-for-powers.md)
- [Universal lossless shortening is impossible](universal-lossless-shortening-is-impossible.md)
